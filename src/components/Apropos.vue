<template>
  <section id="apropos">
    <div class="flexApropos">
      <img id="photoJu" alt="photo Julie" src="../assets/julie.jpg"/>
      <div>
      <h3 id="titreJu">Hello !</h3>
      <p id="textJu">Bienvenue sur mon portfolio codé de mes petits doigts ( je rougis… )<br/>
      Pourquoi ce site ??
      J'ai exercé pendant de nombreuses années, dans diverses agences, le métier de graphiste que j'affectionne beaucoup. <br/>
      Mais voilà… ma curiosité pour le monde digital, l'envie d'apprendre toujours et encore et un gros concours de circonstance m'ont poussée à entreprendre une reconversion.<br/>
      Au terme d'une année de formation où se sont mélés remises en question parfois, épreuves par moment, satisfactions souvent et conviction à chaque instant, ma ténacité m'a permis d'obtenir mon diplôme de développeur web. <br/> 
      C'est donc avec une certaine fierté toute personnelle, que d'Opinel, je suis devenue… couteau suisse !!! ( je vous avais prévenus que je rougissais ^^ )<br/><br/>
      <span id="tobe">To be continued…  </span></p>
    </div>
    </div>
  </section>
</template>

<script>
// @ is an alias to /src


export default {
  name: 'Apropos',
  components: {
    
  }
}
</script>

<style lang="scss">

@import "../sass/main.scss";

#titreJu{
  font-weight: 400;
        font-size: 2rem;
        font-family: $handwritting;
  animation-name: anim-text;
          animation-duration: 2s;
          animation-fill-mode: forwards;
          margin-bottom: 10%;
}

#apropos {
  text-align: justify;
  font-family: $serif;
  line-height: 1.3rem;
  @include mobile{
    width: 100%;
  }


  .flexApropos {
    display: flex;
    flex-direction: row;
    @include mobile{
      flex-direction: column;
    }

    #photoJu {
      max-height: 590px;
      margin-right: 3%;
      animation-name: anim-photo;
      animation-duration: 1.5s;
      animation-fill-mode: forwards;
      opacity: 0;
      z-index: -10;
      @include mobile{
        display: none;
      }
    }

    #textJu {
      font-size: 1rem;
      line-height: 1.5rem;
      animation-name: anim-text;
      animation-duration: 2s;
      animation-fill-mode: forwards;
      
        @include mobile{
        font-size: 0.8rem;
        line-height: 1.5rem;
        width: 100%;

  }
    }
    #tobe{
      font-family: $handwritting;
    }
  }
}



    @keyframes anim-photo {
      0% {
        transform: translate(1000px, 0px);
        opacity: 0;
      }

      // 50% {
      //   transform: translate(500px, 0px);
      //   opacity: 0.5;
      // }
            100% {
        transform: translate(0px, 0px);
        opacity: 1;
      }
    }

    @keyframes anim-text {
      from {
        transform: translate(2830px, 0px);
      }

      to {
        transform: translate(0px, 0px);
      }
    }



</style>
