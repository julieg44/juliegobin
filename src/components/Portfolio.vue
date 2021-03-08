<template >
  <section class="portfolio">
    <Default v-if="portfolioDefault===true"/>
    <Dev v-if="dev===true"/>
    <Graphisme v-if="graphisme===true" />
    <Divers v-if="divers===true" />
  </section>
</template>

<script>
// @ is an alias to /src

import Dev from '@/components/portfolio/Dev.vue';
import Default from '@/components/portfolio/portfolioDefault.vue';
import Graphisme from '@/components/portfolio/Graphisme.vue';
import Divers from '@/components/portfolio/Divers.vue';



export default {
  name: 'Portfolio',
  components: {
    Default, Dev, Graphisme, Divers
  },

  props: {
      portfolioDefault: Boolean,
      dev:Boolean,
      graphisme: Boolean,
      divers: Boolean,
  },
}
</script>

<style lang="scss">

@import "../sass/main.scss";


#align{
    display: flex;
    flex-direction: row;
    align-items: center;
    margin-bottom: 5%;
}

.portfolio {
  position: relative;
    h3 {
        text-align: center;
        font-family: $serif;
        font-weight: 400;
        font-size: 2rem;
        margin-bottom: 2%;
        @include mobile {
          font-size: 1.5rem;
        }
    }
}











</style>
