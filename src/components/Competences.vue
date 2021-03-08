<template>
  <section class="competences">
    <div id="quadrillage-logos"> 
        <div class="logos logoscarre"><img src="../assets/logiciels/html.png" alt="logo HTML"/></div>
        <div class="logos logoscarre"><img src="../assets/logiciels/css-3.png" alt="logo CSS"/></div>
        <div class="logos logoscarre"><img src="../assets/logiciels/sass.png" alt="logo SASS"/></div>
        <div class="logos logoscarre"><img src="../assets/logiciels/js.jpg" alt="logo Javascript"/></div>
        <div class="logos logoslong"><img src="../assets/logiciels/vue.png" alt="logo vue.js"/></div>
        <div class="logos logoslong"><img src="../assets/logiciels/node.png" alt="logo Node"/></div>
        <div class="logos logoslong"><img src="../assets/logiciels/sequelize.png" alt="logo sequelize"/></div>
        <div class="logos logoslong"><img src="../assets/logiciels/express.png" alt="logo express.js"/></div>
        <div class="logos logoslong"><img src="../assets/logiciels/mongodb.jpg" alt="logo mongoDB"/></div>
        <div class="logos logoslong"><img src="../assets/logiciels/MySQL.png" alt="logo MySql"/></div>
        <div class="logos logoscarre"><img src="../assets/logiciels/ID.png" alt="logo InDesign"/></div>
        <div class="logos logoscarre"><img src="../assets/logiciels/AI.png" alt="logo Illustrator"/></div>
        <div class="logos logoscarre"><img src="../assets/logiciels/PS.png" alt="logo Photoshop"/></div>
    </div>
    <!-- <div id="mots"> 
        <img src="../assets/mots.png"/>
    </div> -->
    <div id="mots"> 
        <p>Au delà de mes connaissances techniques ci-dessus, je suis <span class="qualite">curieuse</span> et <span class="qualite">créative</span> de nature, je m'<span class="qualite">adapte facilement</span> aux situations.
          Je prends le temps d’observer afin d’<span class="qualite">analyser au mieux</span> les problématiques et leur trouver la <span class="qualite">solution la plus efficace</span>. 
          Enfin je me plais à <span class="qualite">travailler en équipe</span> et mets toute ma <span class="qualite">bienveillance</span> à sa disposition.
          Je suis <span class="qualite">très très sympa</span> en fait !
        </p>
    </div>
  </section>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Competences',
  components: {
    
  }
}
</script>

<style lang="scss">

@import "../sass/main.scss";

#quadrillage-logos {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  width: 100%;
  margin: auto;
  margin-bottom: 10%;
  @include mobile{
    width: 100%;
    margin: 0;
    }
  .logos {
    width: 100px;
    height: 100px;
    display: flex;
    align-items: center;
    justify-content: center;
    border: 1px solid $grey;
    margin: 2px;
    // @include mobile{
    //   width: 90px;
    //   height: 90px;
    // }

    
    &.logoscarre{
      padding: 23px;
    }
    &.logoslong{
      padding: 10px;
    }
    img {
      width: 100%;      
    }
  }
}
#mots{
  width: 80%;
  @include mobile{
    width: 100%;
  }
  p{
    text-align: left;
  }
  .qualite{
    background-color: black;
    color: $secondColor;
    font-weight: 500;
    margin-left: 2px;
    margin-right: 2px;
    padding-left: 6px;
    padding-right: 6px;
  }
}









</style>
