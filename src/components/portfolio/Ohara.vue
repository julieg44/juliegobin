<template>
    <section class="theme">
    <div class="client">
        <img class="long" src="../../assets/logos/ohara.jpg"/>
    </div>
    <div v-if="grand===false" @click="grand=true" class="boulot">
        <img src="../../assets/ohara-mini.jpg"/>
    </div>

    <div v-if="grand===true" class="full">
        <img src="../../assets/ohara.jpg"/>
        <p @click="grand=false" class="close-full">close</p>
    </div>
<Explicatif titre="Ohara - Agence Loom"
 text1="Déclinaison de maquettes pour le site institutionnel"/>
    </section>
</template>

<script>
// @ is an alias to /src
import Explicatif from '@/components/portfolio/Explicatif.vue';


export default {
  name: 'ohara',
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
