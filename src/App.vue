<template>
  <div id="app">
    <Header/>
    <div class="typer-box">
      <vue-typer :text='["kooijj", "ljlkjl"]' 
        erase-style='backspace' />
    </div>
    <section class="articles__wrapper">
      <Article
        id="article1"
        title="Blick in technologische Zukunft"
        summary="Die Besucher lernen Leonie kennen - eine Sprachassistentin, die neben einer Stimme auch einen digitalen Körper hat."
        excerptHeader="Schlossmuseum: Blick in technologische Zukunft"
        excerpt="Die Besucher lernen Leonie kennen - eine Sprachassistentin, die neben einer Stimme auch einen digitalen Körper hat. Leonie kann nicht nur auf Kommando tanzen, sondern auch Fragen beantworten, etwa über die technologischen Innovationen, die auf uns zukommen, erklärt der Maturant Karsten Köhne. In der HTL Leonding wurde Leonie von Schülern entwickelt."
        imgPath="code.jpeg"
        articlePath="https://ooe.orf.at/news/stories/2957975/?fbclid=IwAR1woeeBFuToOVibSdHlwoRkSXZEZcKXG6wphbcmq9WR9W-F9zebeUEeqo4"
      />

      <Article
        id="article2"
        title="Neues aus der Zukunft"
        summary="Alexa und Siri kennen Sie vermutlich. Aber kennen Sie auch Leonie?"
        excerptHeader="Neues aus der Zukunft"
        excerpt="Alexa und Siri kennen Sie vermutlich. Aber kennen Sie auch Leonie? Die Oö. Zukunftsakademie, ein Think Tank der Oö. Landesregierung, blickt in die Zukunft und stellt im Innovationseck der Dauerausstellung „Technik Oberösterreich“ technologische Entwicklungen der nächsten Jahre, Jahrzehnte, vielleicht auch Jahrhunderte vor."
        imgPath="girl.jpeg"
        articlePath="http://www.landesmuseum.at/de/ausstellungen/detail/techvisionen-neues-aus-der-zukunft.html"
      />

      <Article
        id="article3"
        title="Schlossmuseum wirft einen Blick in die Welt der Zukunft"
        summary="Die neue Sonderausstellung Tech Visionen - Neues aus der Zukunft ist bis 31. März im Innovationseck zu sehen"
        excerptHeader="Welt der Zukunft"
        excerpt="3D-Avatare, ein Gehirn-Computer-Interface, humanoide Roboter, Ganzkörperscanner – die Sonderschau Tech Visionen – Neues aus der Zukunf gibt seit Mittwoch im Linzer Schlossmuseum einen Ausblick auf künftige technologische Entwicklungen. Die in Kooperation mit der Zukunftsakademie – dem Thinktank der Landesregierung – entstandene Schau läuft bis 31. März. Zu sehen ist sie im Innovationseck der Dauerausstellung Technik Oberösterreich."
        imgPath="leonie_first_playcanvas_test.png"
        articlePath="https://www.nachrichten.at/nachrichten/kultur/das-schlossmuseum-wirft-einen-blick-in-die-welt-der-zukunft;art16,3090778"
      />

      <Article
        id="article4"
        title="TechVisionen – Neues aus der Zukunft"
        summary="Eine Sonderschau TechVisionen – Neues aus der Zukunft"
        excerptHeader="TechVisionen – Neues aus der Zukunft"
        excerpt="Der Avatar Leonie als 3D-Hologramm der HTL Leonding wurde für die Ausstellung trainiert, Fragen zu aktuellen Studien der Zukunftsakademie zu beantworten. Eine Sonderschau TechVisionen – Neues aus der Zukunft gibt seit Mittwoch im Bereich der Technik-Dauerausstellung im Linzer Schlossmuseum einen Ausblick auf künftige Technologien."
        imgPath="meeting.jpeg"
        articlePath="https://derstandard.at/2000095788518/Neues-aus-der-Zukunft-im-Linzer-Schlossmuseum"
      />
    </section>

    <Footer></Footer>

    <!-- <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App yeeeeaaaa"/>-->
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
import Header from "./components/Header.vue";
import Article from "./components/Article.vue";
<<<<<<< HEAD
import Footer from "./components/Footer.vue";

=======
import { VueTyper } from 'vue-typer'
//import Typer from "./components/Typer.vue";
>>>>>>> 51cb73bd259e14d9999ec6a96fbea38819bbd62b

export default {
  name: "app",
  components: {
    //HelloWorld,
    Header,
    Article,
<<<<<<< HEAD
    Footer
=======
    VueTyper
>>>>>>> 51cb73bd259e14d9999ec6a96fbea38819bbd62b
  }
};
</script>

<style lang="css">
#app {
  /* font-family: 'Avenir', Helvetica, Arial, sans-serif; */
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center;
    color: #2c3e50;
    margin-top: 60px; */
  display: flex;
  flex-direction: column;
  flex-wrap: wrap;
}
.articles__wrapper {
  margin: 0 auto;
  margin-top: 6rem;
  /* margin-left: 11.5rem; */
  display: grid;
  grid-gap: 8vw;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: auto;
}

.typer-box {
  position: relative;
  top: -20%;
}

@media screen and (max-width: 960px) {
  .articles__wrapper {
    grid-template-columns: 1fr;
  }
}
</style>
