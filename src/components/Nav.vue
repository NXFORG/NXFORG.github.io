<template>
<div id="app">
 <v-app>
  <div>
    <v-app-bar color="blue-grey darken-3" dense dark>
    <v-app-bar-nav-icon @click="drawer = true"></v-app-bar-nav-icon>
    <v-toolbar-title>{{title}}</v-toolbar-title>
    <v-spacer> </v-spacer>
    </v-app-bar>
    <v-navigation-drawer v-model="drawer" absolute temporary>
        <v-list>
      <v-list-item v-for="n in icons" :key="n" @click="() => {}" :href="n.url">
       <v-list-item-icon>
        <v-icon>{{n.ico}}</v-icon>
       </v-list-item-icon><v-list-item-title>{{ n.label }}</v-list-item-title>
      </v-list-item>
     </v-list>
    </v-navigation-drawer>
  </div>
 </v-app>
</div>
</template>

<script>
export default {
  name: 'NavBar',
  props: {
    title: String
  },
      data: () => ({
       drawer: false,
       group: null,
       icons: [
       {
         ico: 'mdi-facebook',
         url: 'https://www.facebook.com/christopher.anstead',
         label: 'Facebook',
       },
       {
         ico: 'mdi-twitter',
         url: 'https://twitter.com/NX_FORG',
         label: 'Twitter',
       },
       {
         ico: 'mdi-linkedin',
         url: 'https://www.linkedin.com/in/christopher-anstead-7b2072a8/',
         label: 'LinkedIn',
       },
       {
         ico: 'mdi-code-greater-than-or-equal',
         url: 'https://github.com/NXFORG',
         label: 'GitHub',
       },
       ]
     })
    }
</script>