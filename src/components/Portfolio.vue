<template>
  <div id="portfolio">
    <Header />
    <ProgrammingSkills />
  </div>
</template>

<script>

import Header from './Portfolio/Header.vue'
import ProgrammingSkills from './Portfolio/ProgrammingSkills.vue'

export default {

  name: 'Portfolio',

  components: {
    Header,
    ProgrammingSkills
  },

  data () {
    return {

    }
  }
}
</script>

<style lang="css" scoped>
</style>