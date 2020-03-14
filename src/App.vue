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
  },
  created: () => {
    document.title = 'My Portfolio'
  }
}
</script>

<style>

:root {
  --bg-color: #fffffa;
  --color1: #6b95e3;
  --color2: #84a5e3;
  --color3: #5079c7;
}

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Roboto', sans-serif;
  color: #333;
  height: 5000px;
  background-color: var(--bg-color);
}

a {
  color: #333; 
}

</style>
