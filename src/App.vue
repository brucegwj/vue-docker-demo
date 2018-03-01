<template>
  <div id="app">
    <img src="./assets/logo.png">
    <!-- <top-gitment :options="options" v-if="options"></top-gitment> -->
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      options: {
        id: 'article id',
        owner: 'Your GitHub ID',
        repo: 'The repo to store comments',
        oauth: {
          client_id: 'Your client ID',
          client_secret: 'Your client secret'
        }
      }
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
