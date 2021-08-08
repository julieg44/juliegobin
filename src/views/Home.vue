<template>
<div>
<!-- <Soon v-if="soon===true"/> -->
  <div class="home">
    <Entete  @affichageHome="showHome()"/>
    <div class="corps">
    <Nav 
    @affichageNav="showNav()"
    @fermetureNav="hideNav()"
    @affichagePortfolio="showPortfolio()"
    @affichageDev="showDev()"
    @affichageGraphisme="showGraphisme()"
    @affichageAutre="showAutre()"
    @affichageCV="showCV()" 
    @affichageContact="showContact()" 
    @affichageCompetences="showCompetences()" 
    :competences="competences"
    :apropos="apropos"
    :contact="contact"
    :portfolio="portfolio"
    :mobiledevice="mobiledevice"
    :burger="burger"
    :navopen="navopen"
    :cv="cv"/>

    <div class="contenu">
    <Apropos v-if="apropos===true"/>
    <Portfolio v-if="portfolio===true"
    :portfolioDefault="portfolioDefault" 
    :dev="dev"
    :graphisme="graphisme"
    :divers="divers"
    @closeFooter="fermerFooter()"/>
    <Contact v-if="contact===true"/>
    <CV v-if="cv===true"/>
    <Competences v-if="competences===true"/>
    </div>
    </div> 
    <Footer :navopen="navopen"/> 
  </div>
</div>
</template>

<script>
// @ is an alias to /src
// import Soon from '@/components/Soon.vue';

import Entete from '@/components/Entete.vue';
import Nav from '@/components/Nav.vue';
import Footer from '@/components/Footer.vue';
// import Prez from '@/components/Prez.vue';
import Portfolio from '@/components/Portfolio.vue';
import Contact from '@/components/Contact.vue';
import Apropos from '@/components/Apropos.vue';
import Competences from '@/components/Competences.vue';
import CV from '../components/CV.vue';



export default {
  name: 'Home',
  components: {
     Entete, Nav, Footer, Portfolio, Contact, Apropos, Competences, CV
    
  },

  data(){
    return {
      // soon: false,
      footer:true,
      mobiledevice:false,
      burger:true,
      navopen:false,
      prez: false,
      portfolio: false,
      apropos: true,
      contact: false,
      competences: false,
      dev: false,
      graphisme: false,
      divers: false,
      cv: false,
    }
  },
  methods:{
    showNav(){
      return this.navopen=true, this.burger=false, this.dev=false, this.portfolio=false, this.prez=false, this.apropos=false, this.contact=false, this.competences=false, this.portfolioDefault=false, this.cv=false
    },
    hideNav(){
      return this.navopen=false, this.burger=true, this.dev=false, this.portfolio=false, this.prez=false, this.apropos=true, this.contact=false, this.competences=false, this.portfolioDefault=false, this.cv=false
    },

    showHome(){
      return this.apropos=true, this.portfolio=false, this.portfolioDefault=false, this.dev=false, this.graphisme=false, this.divers=false, this.contact=false, this.competences=false, this.cv=false, this.navopen=false, this.burger=true
    },
    showPortfolio(){
      return this.portfolio=true, this.portfolioDefault=true, this.dev=false, this.graphisme=false, this.divers=false, this.prez=false, this.apropos=false, this.contact=false, this.competences=false, this.navopen=true, this.burger=false, this.cv=false
    },
    showDev(){
      return this.dev=true, this.graphisme=false, this.divers=false, this.portfolioDefault=false, this.navopen=false, this.burger=true
    },
    showGraphisme(){
      return this.dev=false, this.graphisme=true, this.divers=false, this.portfolioDefault=false, this.navopen=false, this.burger=true
    },
    showAutre(){
      return this.dev=false, this.graphisme=false, this.divers=true, this.portfolioDefault=false, this.navopen=false, this.burger=true
    },
    showCV(){
      return this.cv=true, this.dev=false,this.portfolio=false, this.prez=false, this.apropos=false, this.contact=false, this.competences=false, this.portfolioDefault=false, this.navopen=false, this.burger=true
    },
    showContact(){
      return this.dev=false,this.portfolio=false, this.prez=false, this.apropos=false, this.contact=true, this.competences=false, this.portfolioDefault=false, this.navopen=false, this.burger=true, this.cv=false
    },
    showCompetences(){
      return this.dev=false, this.portfolio=false, this.prez=false, this.apropos=false, this.contact=false, this.competences=true, this.portfolioDefault=false, this.navopen=false, this.burger=true, this.cv=false
    },
  },

  // created(){
  //   console.log(window.innerWidth)
  //   if (window.innerWidth < 600){
  //     console.log("coucou")
  //     return this.soon=true, this.mobiledevice=false, this.burger=false, this.apropos=false
  //   } else {
  //     console.log("raté")
  //   }
  // }

    created(){
    console.log(window.innerWidth)
    if (window.innerWidth < 600){
      console.log("coucou")
      return this.mobiledevice=true
    } else {
      console.log("raté")
    }
  }

  

}
</script>

<style lang="scss">
@import "../sass/main.scss";
.home{
  background-image: url('../assets/fond.svg');
  background-repeat: no-repeat;
  background-position: bottom;
  padding-bottom:20px;
  @include mobile{
    background-image: none;
    width: 90%;
    margin: auto;
  }
}

.corps{
  max-width: 980px;
  margin: auto;
  margin-top: 5%;
  display: flex;
  flex-direction: row;
  // position: relative;
  z-index: 10;
  @include mobile{
    width: 100%;
    flex-direction: column;
    // position: relative;
  }
}
.contenu{
  width: 68%;
  margin-bottom: 5%;
  // display: flex;
  // align-items: center;
  // justify-content: center;
  @include mobile{
    margin-left: 0;
    margin-top: 10%;
    // position: relative;
    width: 100%;
  }
}
</style>
