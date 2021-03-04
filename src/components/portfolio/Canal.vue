<template>
    <section class="theme">
    <div class="client">
        <img class="long" src="../../assets/logos/canal.jpg"/>
    </div>

    <div v-if="grand===false" @click="grand=true" class="boulot">
        <img src="../../assets/canal/GIF_CANAL.gif"/>
    </div>

    <div v-if="grand===true" class="full">
        <img src="../../assets/canal/GIF_CANAL.gif"/>
        <p @click="grand=false" class="close-full">close</p>
    </div>
    <div class="boulot">
        <img src="../../assets/canal/landing-canal.jpg"/>
    </div>


<Explicatif titre="Canal+ business - Agence Loom"
 text1="Déclinaisons de maquettes pour le site"
 text2="Création et intégration de landing page et emails"/>
 
    </section>
</template>

<script>
// @ is an alias to /src
import Explicatif from '@/components/portfolio/Explicatif.vue';


export default {
  name: 'canal',
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

.boulot{
    // display: flex;
    // flex-direction: row;
    // justify-content: space-around;
    width: 100%;
    img{
        width: 100%;
    }
}









</style>
