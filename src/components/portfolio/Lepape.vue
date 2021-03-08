<template>
    <section class="theme">
    <div class="client">
        <img class="long" src="../../assets/logos/lepape.png" alt="logo Lepape"/>
    </div>
    <div class="boulot">
        <img src="../../assets/catalogue/MES.png" alt="ecran Lepape"/>
    </div>
    <div class="client">
        <img class="court" src="../../assets/logos/bbArt.jpg" alt="logo BabyArt"/>
    </div>
    <div class="boulot">
        <img src="../../assets/catalogue/MES.jpg" alt="ecran BabyArt"/>
    </div>
<Explicatif titre="Catalogues - Agence Loom"
 text1="Mise en page et déclinaisons selon DA établie"/>
 
    </section>
</template>

<script>
// @ is an alias to /src
import Explicatif from '@/components/portfolio/Explicatif.vue';


export default {
  name: 'lepape',
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
