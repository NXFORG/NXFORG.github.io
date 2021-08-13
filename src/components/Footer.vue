<template>
    <v-footer dark padless>
     <v-card class="flex" flat tile>
       <v-card-title class="blue-grey darken-3">
         <strong class="subheading">{{title}}</strong>
         <v-spacer></v-spacer>
       <v-tooltip top v-for="icon in icons" :key="icon">
        <template v-slot:activator="{ on, attrs }">
          <v-btn  class="mx-4" dark icon :href="icon.url" v-bind="attrs" v-on="on">
            <v-icon size="24px" :to="icon.url">
             {{ icon.ico }}
            </v-icon>
          </v-btn>
        </template>
        <span>{{icon.label}}</span>
       </v-tooltip>
       </v-card-title>
       <v-card-text class="blue-grey darken-4 py-2 white--text text-center">
         {{ new Date().getFullYear() }} — <strong>Chris Anstead</strong>
       </v-card-text>
     </v-card>
   </v-footer>
</template>

<script>
export default {
  name: 'pageFooter',
  props: {
      title: String
  },
  data: () => ({
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