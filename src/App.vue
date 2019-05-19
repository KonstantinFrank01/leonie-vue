<template>
  <div id="app">
    <Header />
    <Article 
      title="Blick in technologische Zukunft"
      summary="lkfafagsgagaa"
      excerptHeader="jlkdlsjlsjd"
      excerpt="jlskdlsjdkls"
    />
    <!-- <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App yeeeeaaaa"/> -->
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
import Header from './components/Header.vue'
import Article from './components/Article.vue'

export default {
  name: 'app',
  components: {
    //HelloWorld,
    Header,
    Article
  }
}
</script>

<style lang="css">
/* #app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
} */
</style>
