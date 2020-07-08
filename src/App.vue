<template>
  <div id="app">
    hello world
    <p>{{ message }}</p>
  </div>
</template>

<script>
export default {
  name: 'App',
  components: {},
  computed: {
    message: function () {
      return this.$store.getters.message;
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
