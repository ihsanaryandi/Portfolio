<template>
  <div id="app">
    <Portfolio />
  </div>
</template>

<script>
import Portfolio from './components/Portfolio.vue'

export default {
  name: 'App',
  components: {
    Portfolio
  }
}
</script>

<style>

:root {
  --bg-color: #333;
  --color1: #eee;
  --color2: #bbb;
  --color3: #aaa;
}

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  background-color: var(--bg-color);
  font-family: 'Roboto', sans-serif;
  color: var(--color1);
}

</style>
