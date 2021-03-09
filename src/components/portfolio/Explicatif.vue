<template>
    <div>
        <div class="icon-explicatif" @click="explicatif=true" @mouseleave="explicatif=false"><p>Ce que j'ai fait ?</p>
        </div>
        <div class="text-explicatif"  v-if="explicatif===true">
            <h4><slot>{{titre}}</slot></h4>
            <ul class="listeExplication">
                <li v-if="text1"><slot>{{text1}}</slot></li>
                <li v-if="text2"><slot>{{text2}}</slot></li>
                <li v-if="text3"><slot>{{text3}}</slot></li>
                <li v-if="text4"><slot>{{text4}}</slot></li>
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
  data(){
      return{
          explicatif:false
      }
  },
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



    .text-explicatif {
        padding: 4%;
        position: absolute;
        background-color: $secondColor;
        top: 300px;
        width: 200%;
        @include mobile {
            width: 100%;
        }

        h4 {
            font-family: $serif;
            font-weight: 700;
            font-size: 1.2rem;
            color: $firstColor;
            margin-bottom: 2%;
            @include mobile{
                font-size: 1rem;
            }
        }

        .listeExplication {
            font-family: $serif;
            font-weight: 200;
            font-size: 1rem;
            color: $firstColor;
            @include mobile{
                font-size: 0.8rem;
            }
        }
    }

    .icon-explicatif {
        // display: flex;
        // width: 8%;
        // height: 40px;
        // flex-direction: row;
        position: absolute;
        padding: 0px 2% 0px 2%;
        top: 10px;
        right: 0px;
        background-color: $firstColor;
        align-items: center;
        cursor: pointer;
        @include mobile {
            top: 0px;
        }

        p {
            text-align: center;
            font-size: 1.2rem;
            color:$secondColor;
            font-weight: 400;
            font-family: $serif;
            @include mobile{
                font-size: 1rem;
            }
        }
    }










</style>
