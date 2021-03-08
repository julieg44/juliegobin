<template>
    <div id="graphisme">
        <div @click="affPageIntro()"  id="align">
            <h3 >Graphisme</h3>
            <p class="back" v-if="mget===true || moulin===true || pozzo===true || canal===true || irm===true || arc===true || logicmax===true || lepape===true || ohara===true || sdmo===true || sarre===true">   back</p>
            <!-- <Next @One="affPageMget()" @Two="affPageIrm()" @Three="affPageMoulin()" @Four="affPageArc()" @Five="affPageSarre()" @Six="affPageOhara()" @Seven="affPageLepape()"  @Eight="affPageCanal()" @Nine="affPageSdmo()"  @Ten="affPagePozzo()" @Eleven="affPageLogicmax()"/> -->
        </div>
        <Intro v-if="intro===true" @One="affPageMget()" @Two="affPageIrm()" @Three="affPageMoulin()" @Four="affPageArc()" @Five="affPageSarre()" @Six="affPageOhara()" @Seven="affPageLepape()"  @Eight="affPageCanal()" @Nine="affPageSdmo()"  @Ten="affPagePozzo()" @Eleven="affPageLogicmax()"/>
        <Mget v-if="mget===true" />
        <Moulin v-if="moulin===true" />
        <Irm v-if="irm===true"/>
        <Arc v-if="arc===true"/>
        <Sarre v-if="sarre===true"/>
        <Ohara v-if="ohara===true"/>
        <Lepape v-if="lepape===true"/>
        <Canal v-if="canal===true"/>
        <Sdmo v-if="sdmo===true"/>
        <Pozzo v-if="pozzo===true"/>
        <Logicmax v-if="logicmax===true"/>
    </div>
</template>

<script>
// @ is an alias to /src
// import Next from '@/components/portfolio/Next.vue';
import Intro from '@/components/portfolio/GraphismeIntro.vue';

import Moulin from '@/components/portfolio/Moulin.vue';
import Mget from '@/components/portfolio/MGET.vue';
import Irm from '@/components/portfolio/Irm.vue';
import Arc from '@/components/portfolio/Arc.vue';
import Sarre from '@/components/portfolio/Sarre.vue';
import Ohara from '@/components/portfolio/Ohara.vue';
import Lepape from '@/components/portfolio/Lepape.vue';
import Canal from '@/components/portfolio/Canal.vue';
import Sdmo from '@/components/portfolio/SDMO.vue';
import Pozzo from '@/components/portfolio/Pozzo.vue';
import Logicmax from '@/components/portfolio/Logicmax.vue';





export default {
  name: 'graphisme',
  components: {
    Intro, Moulin, Mget, Irm, Arc, Sarre, Ohara, Lepape,Canal, Sdmo,Pozzo,Logicmax, 
  },
  props:{
    introGraphisme: Boolean
  },

  data() {
      return {
          intro:true,
          moulin: false,
          mget: false,
          irm: false,
          arc: false,
          sarre: false,
          ohara: false,
          lepape:false,
          canal: false,
          sdmo:false,
          pozzo:false,
          logicmax:false
      }
  },

computed:{

},

  methods: {
      affPageIntro() {
          return this.intro=true, this.logicmax=false, this.pozzo=false, this.sdmo=false, this.canal=false, this.lepape=false, this.ohara = false, this.sarre = false, this.arc = false, this.moulin = false, this.mget = false, this.irm = false
      },
      affPageMget() {
          return this.mget = true, this.irm = false, this.moulin = false, this.arc = false, this.sarre = false, this.ohara = false, this.lepape=false, this.canal=false,this.sdmo=false, this.pozzo=false, this.pozzo=false, this.logicmax=false, this.intro=false
      },
      affPageIrm() {
          return this.irm = true, this.mget = false, this.moulin = false, this.arc = false, this.sarre = false, this.ohara = false, this.lepape=false, this.canal=false,this.sdmo=false, this.pozzo=false, this.pozzo=false, this.logicmax=false, this.intro=false
      },
      affPageMoulin() {
          return this.moulin = true, this.mget = false, this.irm = false, this.arc = false, this.sarre = false, this.ohara = false, this.lepape=false, this.canal=false,this.sdmo=false, this.pozzo=false, this.pozzo=false, this.logicmax=false, this.intro=false
      },
      affPageArc() {
          return this.arc = true, this.moulin = false, this.mget = false, this.irm = false, this.sarre = false, this.ohara = false, this.lepape=false, this.canal=false, this.sdmo=false, this.pozzo=false, this.pozzo=false, this.logicmax=false, this.intro=false
      },
      affPageSarre() {
          return this.sarre = true, this.arc = false, this.moulin = false, this.mget = false, this.irm = false, this.ohara = false, this.lepape=false, this.canal=false, this.sdmo=false, this.pozzo=false, this.pozzo=false, this.logicmax=false, this.intro=false
      },
      affPageOhara() {
          return this.ohara = true, this.sarre = false, this.arc = false, this.moulin = false, this.mget = false, this.irm = false, this.lepape=false, this.canal=false,this.sdmo=false, this.pozzo=false, this.pozzo=false, this.logicmax=false, this.intro=false
      },
        affPageLepape() {
          return this.lepape=true, this.ohara = false, this.sarre = false, this.arc = false, this.moulin = false, this.mget = false, this.irm = false, this.canal=false, this.sdmo=false, this.pozzo=false, this.pozzo=false, this.logicmax=false, this.intro=false
      },
        affPageCanal() {
          return this.canal=true, this.lepape=false, this.ohara = false, this.sarre = false, this.arc = false, this.moulin = false, this.mget = false, this.irm = false,this.sdmo=false, this.pozzo=false, this.pozzo=false, this.logicmax=false, this.intro=false
      },
        affPageSdmo() {
          return this.sdmo=true, this.canal=false, this.lepape=false, this.ohara = false, this.sarre = false, this.arc = false, this.moulin = false, this.mget = false, this.irm = false, this.pozzo=false, this.pozzo=false, this.logicmax=false, this.intro=false
      },
        affPagePozzo() {
          return this.pozzo=true, this.sdmo=false, this.canal=false, this.lepape=false, this.ohara = false, this.sarre = false, this.arc = false, this.moulin = false, this.mget = false, this.irm = false, this.logicmax=false, this.intro=false
      },
        affPageLogicmax() {
          return this.logicmax=true, this.pozzo=false, this.sdmo=false, this.canal=false, this.lepape=false, this.ohara = false, this.sarre = false, this.arc = false, this.moulin = false, this.mget = false, this.irm = false, this.intro=false
      },
  }
}
</script>

<style lang="scss">

@import "../../sass/main.scss";
#graphisme{
  cursor: pointer;
  .back{
    margin-left: 3%;
    border: 1px solid $thirdColor;
    // background-color: $thirdColor;
    color: $thirdColor;
    padding: 0 2% 2% 2%;
    height: 25px;
    line-height: 1.5rem;
  }
}

.theme {
  position: relative;
    .client {
        display: flex;
        flex-direction: row;
        align-items: center;
        margin-bottom: 5%;
        border-bottom: 1px solid black;
        h3 {
            width: 30%;
            height: 35px;
            font-size: 1rem;
            background-color: #000;
            color: #ecd1d6;
            text-align: center;
            margin-right: 5%;
            padding-top: 1%;
        }
        .court{
            margin-bottom: 3%;
            max-width: 45%;
            max-height: 95px;
        }
        .long{
            margin-bottom: 3%;
            max-width: 45%;
            max-height: 75px;
        }
    }
}

    .full{
      display: flex;
      flex-direction: row;
      justify-content: space-between;
      position: absolute;
      top: 0;
      left: 0;
      background-color: #fff;
      width: 130%;
      margin-left: -10%;
      margin-top: -18%;
      padding: 3%;
      z-index: 8;
      img{
        width: 95%;
      }
      .close-full{
            background-color: #ecd1d6;
    font-weight: 900;
    font-size: 1.2rem;
    padding: 10px;
    line-height: 1;
    color: #000;
    height: 35px;
    text-align: center;
    font-family: "Montserrat", sans-serif;
      }
    }




</style>
