<template>
<section class="theme">
    <div class="client">
        <!-- <h3>MGET</h3> -->
        <img class="long" src="../../assets/logos/MGET_Logo.jpg"  alt="logo MGET"/>
    </div>
        <div v-if="grand===false" @click="grand=true" class="boulot">
        <img src="../../assets/MGET.png" alt="ecran MGET"/>
    </div>

    <div v-if="grand===true" class="full">
        <img src="../../assets/MGET.png" alt="ecran MGET"/>
        <p @click="grand=false" class="close-full">close</p>
    </div>
<Explicatif titre="MGET campagne 'et moi ça va?' - Agence Loom"
 text1="Déclinaisons de maquettes pour le site de la campagne" 
 text2="Mise en page de divers supports Print"/>
</section>
</template>

<script>
// @ is an alias to /src
import Explicatif from '@/components/portfolio/Explicatif.vue';


export default {
  name: 'MGET',
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
    width: 100%;
    img{
        width: 100%;
    }
}









</style>
