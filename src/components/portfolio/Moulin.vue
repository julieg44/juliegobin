<template>

    <section class="theme">
    <div class="client">
        <h3>Fête du Moulin</h3>
    </div>
    <div class="boulotTwo">
        <img src="../../assets/moulin1.jpg" alt="ecran moulin"/>
        <img src="../../assets/moulin.png" alt="ecran moulin"/>
    </div>
<Explicatif titre="Fête du Moulin - Projet personnel"
 text1="Création du visuel"/>
    </section>
</template>

<script>
// @ is an alias to /src
import Explicatif from '@/components/portfolio/Explicatif.vue';


export default {
  name: 'moulin',
  components: {
    Explicatif
  }
}
</script>

<style lang="scss">

@import "../../sass/main.scss";

.boulotTwo{
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    width: 100%;
    img{
        width: 45%;
        max-height: 460px;
    }
}










</style>
