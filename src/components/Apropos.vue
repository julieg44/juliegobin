<template>
  <section id="apropos">
    <div class="flexApropos">
      <img id="photoJu" src="../assets/julie.jpg"/>
      <div>
      <h3 id="titreJu">Hello !!!</h3>
      <p id="textJu">Je suis Julie, j'ai 38 ans et je vis à Nantes.<br/>
      Qu'est ce que je fabrique sur une page web ? 
      Je m'explique : J'ai exercé dans diverses agences le métier de graphiste que j'affectionne beaucoup. <br/>
      Mais voilà… crise de la quarantaine approchant (sans doute), 
      l'envie d'apprendre toujours et encore, 
      les opportunités d'expression qu'offrent le monde digital et un petit concours 
      de circonstance m'ont poussé à entreprendre une reconversion. <br/><br/> 
      Me voici donc développeur Web ( junior => merci de votre indulgence ;) prête à me lancer dans de tout nouveaux défis ! </p>
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
  animation-name: anim-text;
          animation-duration: 2s;
          animation-fill-mode: forwards;
          margin-bottom: 6%;
}

#apropos {
  text-align: justify;
  font-family: $serif;
  line-height: 2rem;
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
      width: 35%;
      max-height: 460px;
      margin-right: 3%;
      animation-name: anim-photo;
      animation-duration: 1.5s;
      animation-fill-mode: forwards;
      opacity: 0;
      @include mobile{
        display: none;
      }
    }

    #textJu {
      font-size: 1rem;
      animation-name: anim-text;
      animation-duration: 2s;
      animation-fill-mode: forwards;
      
        @include mobile{
        font-size: 0.8rem;
        line-height: 1.5rem;
        width: 100%;

  }
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
