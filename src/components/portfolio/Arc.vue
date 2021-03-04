<template>
<section class="theme">
    <div class="client">
        <img class="court" src="../../assets/logos/arc.jpg"/>
    </div>
    <div v-if="grand===false" @click="grand=true" class="boulot">
        <img src="../../assets/arc.jpg"/>
    </div>

    <div v-if="grand===true" class="full">
        <img src="../../assets/arc.jpg"/>
        <p @click="grand=false" class="close-full">close</p>
    </div>
<Explicatif titre="Groupe Arc - Agence Loom"
 text1="Déclinaison de maquettes pour le site institutionnel"/>
</section>
</template>

<script>
// @ is an alias to /src
import Explicatif from '@/components/portfolio/Explicatif.vue';


export default {
  name: 'Arc',
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
