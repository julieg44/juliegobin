<template>
<section class="theme">
    <div class="client">
        <h3>Sarré conseils</h3>
    </div>    
    <div v-if="grand===false" @click="grand=true" class="boulot">
        <img src="../../assets/sarre-mini.gif"/>
    </div>

    <div v-if="grand===true" class="full">
        <img src="../../assets/sarre.gif"/>
        <p @click="grand=false" class="close-full">close</p>
    </div>
    <Explicatif titre="Sarré conseil - Agence Loom"
 text1="Intégration du site sous wordpress"/>
</section>
</template>

<script>
// @ is an alias to /src
import Explicatif from '@/components/portfolio/Explicatif.vue';


export default {
  name: 'Sarre',
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
