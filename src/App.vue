<template>
  <div id="app">
    <navigation></navigation>
    <router-view/>
  </div>
</template>

<style lang="scss">
#app {
  @import url('https://fonts.googleapis.com/css2?family=Montserrat&family=Open+Sans:wght@400;700&display=swap');

  body { font-family: 'Open Sans', sans-serif; }

  h1,
  h2,
  h3,
  h4,
  h5,
  h6,
  a {
    font-family: 'Montserrat', sans-serif;
  }

  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>

<script>
import Navigation from './components/Navigation.vue';

export default {
  name: 'App',
  components: {
    navigation: Navigation,
  },
};
</script>
