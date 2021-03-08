<template>
<div id="dev">
        <div id="align">
            <h3>Développement</h3>
            <!-- <NextDev @One="affPageMget()" @Two="affPageIrm()" @Three="affPageMoulin()" /> -->
        </div>    
            <div v-if="grand===false" @click="grand=true" class="boulot">
        <img src="../../assets/PF-dev.png"/>
    </div>

    <div v-if="grand===true" class="fulldev">
        <video src="../../assets/groupomania.mp4" controls autoplay  width="600"></video>
        <p @click="grand=false" class="close-full">X</p>
    </div>
<Explicatif titre="Réseau social Groupomania - Projet d'études"
 text1="Création et gestion de la base de données" 
 text2="Création du design" 
 text3="Création et gestion du Backend et du Frontend" 
 text4="Techno utilisées : MySql - Node - express.js - Vue.js"/>
</div>
</template>

<script>
// @ is an alias to /src
// import NextDev from '@/components/portfolio/NextDev.vue';
import Explicatif from '@/components/portfolio/Explicatif.vue';



export default {
  name: 'Dev',
  components: {
     Explicatif
  },
      data(){
    return{
      grand:false
    }
  }
}
</script>

<style lang="scss">

@import "../../sass/main.scss";

// #dev {
//     h3 {
//         text-align: center;
//         font-family: $serif;
//         font-weight: 400;
//         font-size: 2rem;
//     }

    .signe {
        color: $secondColor;
        font-size: 15rem;
        font-weight: 900;
        opacity: 0.5;
    }

        .fulldev{
      display: flex;
      flex-direction: row;
      justify-content: space-between;
      position: absolute;
      top: 0;
      left: 0;
      background-color: #fff;
      width: 100%;
      border: 1px solid $grey;
    //   margin-left: -20%;
    //   margin-top: -8%;
      padding: 3%;
      z-index: 8;
      video{
        width: 100%;
        margin-right: 5%;
        max-height: 500px;
      }
      .close-full{
        background-color: $secondColor;
        font-weight: 900;
        font-size: 1.5rem;
        color: $firstColor;
        width: 30px;
        height:30px;
        text-align: center;
        font-family: $sansserif;
      }
    }









</style>
