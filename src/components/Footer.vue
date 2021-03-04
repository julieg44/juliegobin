<template>
  <footer>
    <p>Développeur Web <span class="esperluette">&</span> Graphiste</p>
    <div class="filet"></div>
    <div class="frise"><img src="../assets/frise.png"></div>
  </footer>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Footer',
  components: {
    
  },

  props:{
    navopen: Boolean,
    grand:Boolean
  },

  // methods:{
  //   hideFooter(){
  //     return this.grand=false
  //   }
  // }
}
</script>

<style lang="scss">

@import "../sass/main.scss";

footer {
    // margin-top: 3%;
    margin-bottom: 4%;
    width: 66%;
    margin-left: 40%;
    // position: relative;
    // top: 2000px;
    animation-name: anim-footer;
    animation-duration: 1.5s;
    animation-fill-mode: forwards;
    // transition: transform 2s cubic-bezier(.25, .1, .25, 1);
    // transform: translate(0px, -2000px);
    @include mobile{
      display: none;
    }

    .filet {
        height: 2px;
        width: 100%;
        background-color: $thirdColor;
        margin-bottom: 1%;
        @include mobile{
          display: none;
        }
    }

    p {
        font-family: $serif;
        font-size: 1.8rem;
        font-weight: 200;
        text-align: left;
        max-width: 980px;
        color: $thirdColor;

        .esperluette {
            font-size: 3rem;
            font-weight: 400;
            text-align: left;
            max-width: 980px;
            margin: auto;
            color: $secondColor;
            @include mobile{
              font-size: 2rem;
            } 
        }
        @include mobile{
          font-size: 1.4rem;
          width: 110%;
        }
    }
    @include mobile{
      margin-left: 0;
      margin-top: 0;
    }
}
.frise{
  @include mobile{
    display: none;
  }
}


@keyframes anim-footer{
    from {
        transform: translate(0px, 2000px);
    }
    to {
        transform: translate(0px, 0px);
    }
}





</style>
