<template>
    <div class="explicatif" >
        <div class="icon-explicatif" @click="explicatif=true"><p>?</p></div>
        <div class="text-explicatif">
            <h4><slot>{{titre}}</slot></h4>
            <ul class="listeExplication">
                <li><slot>{{text1}}</slot></li>
                <li><slot>{{text2}}</slot></li>
                <li><slot>{{text3}}</slot></li>
                <li><slot>{{text4}}</slot></li>
            </ul>
        </div>
    </div>
</template>


<script>
// @ is an alias to /src


export default {
  name: 'Explicatif',
  components: {
  },
//   data(){
//       return{
//           explicatif:false
//       }
//   },
    props:{
      titre:{ type:String, required:true},
      text1:{ type:String},
      text2:{ type:String},
      text3:{ type:String},
      text4:{ type:String}
  }
}
</script>

<style lang="scss">

@import "../../sass/main.scss";

.explicatif {
    display: flex;
    width: 8%;
    flex-direction: row;
    position: absolute;
        padding: 2%;
    top: 0px;
    right: 0px;
    background-color: $firstColor;
    align-items: center;
    &:hover{
                padding: 4%;

            width: 200%;
        right: 0px;
        background-color: $secondColor;
        top:240px;
        left: 0px;
        .text-explicatif{
            display: block;
        }
        .icon-explicatif{
            display: none;
        }
    }

    .text-explicatif {
display: none;
    width: 200%;

        h4 {
            font-family: $serif;
            font-weight: 700;
            font-size: 1.2rem;
            color: $firstColor;
            margin-bottom: 2%;
        }

        .listeExplication {
            font-family: $serif;
            font-weight: 200;
            font-size: 1rem;
            color: $firstColor;
        }
    }

    .icon-explicatif {
            text-align: center;

        .fa-question {
            font-size: 3rem;
            color: #fff;
            font-weight: 100;
        }
                p {
            font-size: 3rem;
            color: #fff;
            font-weight: 400;
        }
    }
}









</style>
