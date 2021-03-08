<template>
<div id="nav">
    <div id="burger" v-if="burger===true && mobiledevice===true " @click="openNav()">
      <img src="../assets/burger.svg" alt="menu burger"/>
      <div>
        <p>Développeur Web <span class="esperluette">&</span> Graphiste</p>
      </div>
    </div>
    <nav>
      <ul v-show="navopen===true || mobiledevice===false">
        <li v-if="competences===true"><div class="open" @click="openCompetences()"><h2>Compétences</h2></div></li>
        <li v-else><div class="close competences" @click="openCompetences()"><h2>Compétences</h2></div></li>
        
        <li v-if="portfolio===true"><div class="open" @click="openPortfolio"><h2>Portfolio</h2></div>        
          <div class="sousmenu">
            <ul>
              <li @click="openDev()"><p class="sousmenutext">Développement</p></li>
              <li @click="openGraphisme()"><p class="sousmenutext">Graphisme</p></li>
              <li @click="openAutre()"><p class="sousmenutext">Mais aussi…</p></li>
            </ul>
          </div>
        </li>
        <li v-else><div class="close portfolio" @click="openPortfolio()"><h2>Portfolio</h2></div></li>

        <li v-if="cv===true"><div class="open" @click="openCV()"><h2>Mon CV</h2></div></li>
        <li v-else><div class="close apropos" @click="openCV()"><h2>Mon CV</h2></div></li>
        
        <li v-if="contact===true"><div class="open" @click="openContact()"><h2>Contact</h2></div></li>
        <li v-else><div class="close contact" @click="openContact()"><h2>Contact</h2></div></li>
        <li><div class="close closeMenu" @click="closeNav()"><img src="../assets/close.svg"/></div></li>
      </ul>
    </nav>
</div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Nav',
  components: {

  },

  props:{
    competences : Boolean,
    portfolio : Boolean,
    cv : Boolean,
    contact : Boolean,
    burger : Boolean,
    navopen :Boolean,
    mobiledevice : Boolean,
    apropos : Boolean
  },
  methods: {
    openPortfolio() {
      this.$emit('affichagePortfolio')
    },
    openCV() {
      this.$emit('affichageCV')
    },
    openContact() {
      this.$emit('affichageContact')
    },
    openCompetences() {
      this.$emit('affichageCompetences')
    },
    openDev() {
      this.$emit('affichageDev')
    },
    openGraphisme() {
      this.$emit('affichageGraphisme')
    },
    openAutre() {
      this.$emit('affichageAutre')
    },
    openNav(){
      this.$emit('affichageNav')
    },
    closeNav(){
      this.$emit('fermetureNav')
    }
  },
}
</script>

<style lang="scss">

@import "../sass/main.scss";


#nav {
  width: 27%;
  margin-right: 5%;
  // position: relative;
  // top: -430px;
    top: 0px;

  animation-name: anim-nav;
  animation-duration: 1.5s;
  animation-fill-mode: forwards;
  @include mobile{
  width: 100%;
  animation: none;
  // position: inherit;
  top: 0;
  }
  #burger{
    display: none;
    @include mobile{
      display: flex;
      animation: none;
      width: 100%;
        img{
          width: 13%;
          margin-right: 2%;
        }
        p {
        font-family: $serif;
        font-size: 0.8rem;
        font-weight: 200;
        text-align: left;
        width: 85%;
        color: $thirdColor;
        line-height: 1.2rem;
        @include mobile{
          font-size: 1.2rem;
        }
        .esperluette {
              font-size: 1.2rem;
              color: $secondColor;
              font-weight: 900;
              @include mobile{
          font-size: 1.4rem;
        }
            }
        }
       
    }
    }
  
  ul {
  padding-left: 0;
}


li{
  list-style-type: none;
    cursor: pointer;

}

.close {
  background-color: $firstColor;
  margin-bottom: 15%;
  height: 35px;
  padding: 1%;
  transition: transform 400ms;
  @include mobile{
    margin-bottom: 7%;
  }

  &:hover {
    transform: scale(1.15);
    background-color: $secondColor;
  }

  &.competences {
    // position: relative;
    // left: -430px;
    transition: transform 400ms;
    // transform: translate(430px, 0px);
    animation-name: anim-competences;
    animation-duration: 1.5s;
    animation-fill-mode: forwards;
    animation-iteration-count: 1;
      &:hover {
    transform: scale(1.15);
    }
    @include mobile{
      animation: none;
            // position: inherit;

    }
  }

  &.portfolio {
    // position: relative;
    // left: -530px;
    transition: transform 1.5s cubic-bezier(.25, .1, .25, 1);
    // transform: translate(530px, 0px);
    animation-name: anim-portfolio;
    animation-duration: 1.5s;
    animation-fill-mode: forwards;
    animation-iteration-count: 1;
        @include mobile{
      animation: none;
            // position: inherit;

    }
  }

  &.apropos {
    // position: relative;
    // left: -630px;
    transition: transform 1.5s cubic-bezier(.25, .1, .25, 1);
    // transform: translate(630px, 0px);
    animation-name: anim-apropos;
    animation-duration: 1.5s;
    animation-fill-mode: forwards;
    animation-iteration-count: 1;
        @include mobile{
      animation: none;
            // position: inherit;

    }
  }

  &.contact {
    // position: relative;
    // left: -730px;
    transition: transform 1.5s cubic-bezier(.25, .1, .25, 1);
    // transform: translate(730px, 0px);
    animation-name: anim-contact;
    animation-duration: 1.5s;
    animation-fill-mode: forwards;
    animation-iteration-count: 1;
        @include mobile{
      animation: none;
      // position: inherit;
    }
  }
    &.closeMenu{
    display: none;
    @include mobile{
      display: block;
      text-align: center;
      img{
        width: 8%;
      }
    }
  }

  h2 {
    font-family: $serif;
    color: $secondColor;
    font-size: 1.3rem;
    font-weight: 300;
    text-align: center;
    transition: transform 400ms;

    &:hover {
      transform: scale(1.15);
      color: $firstColor;
    }
  }
}
.open{
  background-color: $secondColor;
  list-style-type: none;
  margin-bottom: 15%;
  height: 35px;
  padding: 1%;
  @include mobile{
    margin-bottom: 7%;
  }
  h2{
    font-family: $serif;
    color: $firstColor;
    font-size: 1.3rem;
    font-weight: 300;
    text-align: center;
  }
}
  .sousmenu{
    text-align: center;
    margin-bottom: 15%;
    font-family: $serif;
    line-height: 2rem;
    .sousmenutext {
      cursor: pointer;
      &:hover{
      color: $quatreColor;
      font-weight: 700;
      }
    }
  }
}

@keyframes anim-nav{
    from {
        transform: translate(0px, -430px);
    }
    to {
        transform: translate(0px, 0px);
    }
}
@keyframes anim-competences{
    from {
        transform: translate(-430px, 0px);
    }
    to {
        transform: translate(0px, 0px);
    }
}
@keyframes anim-portfolio{
    from {
        transform: translate(-530px, 0px);
    }
    to {
        transform: translate(0px, 0px);
    }
}
@keyframes anim-apropos{
    from {
        transform: translate(-630px, 0px);
    }
    to {
        transform: translate(0px, 0px);
    }
}
@keyframes anim-contact{
    from {
        transform: translate(-730px, 0px);
    }
    to {
        transform: translate(0px, 0px);
    }
}







</style>
