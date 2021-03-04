<template>
    <section class="theme">
    <div class="client">
        <img class="court" src="../../assets/logos/sdmo.jpg"/>
    </div>
    <div class="boulot">
        <img src="../../assets/SDMO/SDMO-landing.jpg"/>
    </div>
<Explicatif titre="SDMO - Agence Loom"
 text1="Création et intégration de landing page"/>
 
    </section>
</template>

<script>
// @ is an alias to /src
import Explicatif from '@/components/portfolio/Explicatif.vue';


export default {
  name: 'sdmo',
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
