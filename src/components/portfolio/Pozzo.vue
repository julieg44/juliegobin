<template>
    <section class="theme">
    <div class="client">
        <img class="court" src="../../assets/logos/pozzo.png" alt="logo pozzo"/>
    </div>
    <div class="boulot">
        <img src="../../assets/pozzo/pozzo.gif" alt="ecran pozzo"/>
    </div>
    <div class="boulot">
        <img src="../../assets/pozzo/POZZO_asset_5.jpg" alt="ecran pozzo"/>
    </div>
<Explicatif titre="Agence Pozzo immobilier - Agence Loom"
    text1="Déclinaison de maquettes pour le site institutionnel"
 text2="Mise en page de divers supports Print"/>
 
    </section>
</template>

<script>
// @ is an alias to /src
import Explicatif from '@/components/portfolio/Explicatif.vue';


export default {
  name: 'pozzo',
  components: {
    Explicatif
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
