<template>
  <div id="app">
    <Header />
    <Article id="article1"
      title="Blick in technologische Zukunft"
      summary="Die Besucher lernen Leonie kennen - eine Sprachassistentin, die neben einer Stimme auch einen digitalen Körper hat."
      excerptHeader="Schlossmuseum: Blick in technologische Zukunft"
      excerpt="Die Besucher lernen Leonie kennen - eine Sprachassistentin, die neben einer Stimme auch einen digitalen Körper hat. Leonie kann nicht nur auf Kommando tanzen, sondern auch Fragen beantworten, etwa über die technologischen Innovationen, die auf uns zukommen, erklärt der Maturant Karsten Köhne. In der HTL Leonding wurde Leonie von Schülern entwickelt."
    />

    <Article id="article2"
      title="Neues aus der Zukunft"
      summary="Alexa und Siri kennen Sie vermutlich. Aber kennen Sie auch Leonie?"
      excerptHeader="Neues aus der Zukunft"
      excerpt="Alexa und Siri kennen Sie vermutlich. Aber kennen Sie auch Leonie? Die Oö. Zukunftsakademie, ein Think Tank der Oö. Landesregierung, blickt in die Zukunft und stellt im Innovationseck der Dauerausstellung „Technik Oberösterreich“ technologische Entwicklungen der nächsten Jahre, Jahrzehnte, vielleicht auch Jahrhunderte vor."
    />

    <Article id="article3"
      title="Schlossmuseum wirft einen Blick in die Welt der Zukunft"
      summary="Die neue Sonderausstellung Tech Visionen - Neues aus der Zukunft ist bis 31. März im Innovationseck zu sehen"
      excerptHeader="Welt der Zukunft"
      excerpt="3D-Avatare, ein Gehirn-Computer-Interface, humanoide Roboter, Ganzkörperscanner – die Sonderschau Tech Visionen – Neues aus der Zukunf gibt seit Mittwoch im Linzer Schlossmuseum einen Ausblick auf künftige technologische Entwicklungen. Die in Kooperation mit der Zukunftsakademie – dem Thinktank der Landesregierung – entstandene Schau läuft bis 31. März. Zu sehen ist sie im Innovationseck der Dauerausstellung Technik Oberösterreich."
    />

    <Article id="article4"
      title="TechVisionen – Neues aus der Zukunft"
      summary="Eine Sonderschau TechVisionen – Neues aus der Zukunft"
      excerptHeader="TechVisionen – Neues aus der Zukunft"
      excerpt="Der Avatar Leonie als 3D-Hologramm der HTL Leonding wurde für die Ausstellung trainiert, Fragen zu aktuellen Studien der Zukunftsakademie zu beantworten. Eine Sonderschau TechVisionen – Neues aus der Zukunft gibt seit Mittwoch im Bereich der Technik-Dauerausstellung im Linzer Schlossmuseum einen Ausblick auf künftige Technologien."
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
