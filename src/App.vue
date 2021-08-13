<template>
  <v-app>
    <NavBar title="Chris Anstead"/>
    <v-main>
      <mainContent title="Hi, I'm Chris" subtitle="I'm a BSc Computer Science graduate from the University of Portsmouth." content="I enjoy working with new technologies and finding ways of how they can improve people's lives. You will usually find me either in a record store, on a long walk somewhere, or experimenting with some new tech."/>
    </v-main>
    <parallax title="About me"/>
    <carousel/>
    <pageFooter title="Follow me on social media"/>
  </v-app>
</template>

<script>
import NavBar from './components/Nav.vue';
import mainContent from './components/Main.vue';
import parallax from './components/Parallax.vue';
import carousel from './components/Carousel.vue';
import pageFooter from './components/Footer.vue';

export default {
  name: 'App',

  components: {
    NavBar,
    mainContent,
    parallax,
    carousel,
    pageFooter
  },

  data: () => ({
    //
  }),
};
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Montserrat&display=swap');

*{
  font-family: 'Montserrat', sans-serif;
}
</style>