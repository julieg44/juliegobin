<template>
    <section class="theme">
    <div class="client">
        <img class="court" src="../../assets/logos/logicmax.png" alt="logo logicmax"/>
    </div>
    <div class="boulot">
        <img src="../../assets/logicmax/logicmax.gif" alt="ecran logicmax"/>
    </div>
    <div class="boulot">
        <img src="../../assets/logicmax/blog_cedric.gif" alt="ecran logicmax"/>
    </div>
    <div class="boulot flex">
    <div class="bann">
        <img src="../../assets/logicmax/bann.gif" alt="ecran logicmax"/>
    </div>
    <div class="mail">
        <img src="../../assets/logicmax/mail.jpg" alt="ecran logicmax"/>
    </div>
    </div>
<Explicatif titre="logicmax - Agence Loom"
    text1="Déclinaison de maquettes pour le site institutionnel"
    text2="Création et intégration d'articles de blog"
    text3="Création et réalisation de bannières animées"
    text4="Création et intégration d'emails"/>

 
    </section>
</template>

<script>
// @ is an alias to /src
import Explicatif from '@/components/portfolio/Explicatif.vue';


export default {
  name: 'logicmax',
  components: {
    Explicatif
  }
}
</script>

<style lang="scss">

@import "../../sass/main.scss";

.boulot {

    width: 100%;
    margin-bottom: 3%;
    &.flex {
        display: flex;
        flex-direction: row;
        justify-content: space-around;
        .bann {
            width: 40%;
        }
        .mail {
            width: 40%;
        }
    }
    img {
        width: 100%;
    }
}









</style>
