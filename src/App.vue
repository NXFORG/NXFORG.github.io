<template>
  <v-app>
    <v-main>
      <NavBar title="Chris Anstead"/>
    </v-main>
  </v-app>
</template>

<script>
import NavBar from './components/Nav.vue';

export default {
  name: 'App',

  components: {
    NavBar
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