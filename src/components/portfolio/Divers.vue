<template>
    <section class="theme">
        <div id="divers">
            <div id="align">
                <h3>Mais aussi…</h3>
            </div>
        </div>

        <div class="client">
            <h3>un peu de peinture… </h3>
        </div>
        <div class="boulot-toiles">
            <div class="toile"><img src="../../assets/divers/toile1.jpg" /></div>
            <div class="toile"><img src="../../assets/divers/toile3.jpg" /></div>
            <div class="toile"><img src="../../assets/divers/toile2.jpg" /></div>
            <!-- <div class="toile"><img src="../../assets/divers/halloween.jpg" /></div> -->
        </div>
        <Explicatif titre="Pratique peinture et… passion tête de mort"
 text1="Dès que le temps me le permet !" />
    </section>
</template>

<script>
// @ is an alias to /src
import Explicatif from '@/components/portfolio/Explicatif.vue';




export default {
  name: 'divers',
  components: {
      Explicatif
  },

  data() {
      return {
          toile1: false,
      }
  },

computed:{

},

  methods:{
      affPageMget(){
          return this.toile1=true
      },
  }
}
</script>

<style lang="scss">

@import "../../sass/main.scss";

.boulot-toiles{
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    flex-wrap: wrap;
    .toile{ 
    width: 45%;    
    img{
        width: 100%;
        margin-bottom: 3%;
    }
    }
}


</style>
