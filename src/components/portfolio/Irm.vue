<template>
    <section class="theme">
    <div class="client">
        <img class="long" src="../../assets/logos/logo-irm.jpg" alt="logo IRM"/>
    </div>

    <div v-if="grand===false" @click="grand=true" class="boulot">
        <img src="../../assets/IRM-mini.png" alt="ecran IRM"/>
    </div>

    <div v-if="grand===true" class="full">
        <img src="../../assets/IRM.png" alt="ecran IRM"/>
        <p @click="grand=false" class="close-full">close</p>
    </div>

<Explicatif v-if="grand===false" titre="IRM - Agence Loom"
 text1="Déclinaison de maquettes pour le site institutionnel"/>
    </section>
</template>

<script>
// @ is an alias to /src
import Explicatif from '@/components/portfolio/Explicatif.vue';


export default {
  name: 'irm',
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
