<template>
  <div id="portfolio">
    <Header />
    <About />
    <Skills />
  </div>
</template>

<script>

// Components
import Header from './Portfolio/Header'
import About  from './Portfolio/About'
import Skills  from './Portfolio/Skills'

export default {

  name: 'Portfolio',

  components: {
    Header,
    About,
    Skills
  },

  data () {
    return {

    }
  }
}
</script>

<style lang="css" scoped>
</style>