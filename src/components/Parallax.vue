<template>
    <v-parallax src="" class="blue-grey darken-4" height="200">
        <v-row align="center" justify="center">
         <v-col class="text-center" cols="12">
          <h1 class="display-1 font-weight-thin mb-4">{{title}}</h1>
         </v-col>
        </v-row>
    </v-parallax>
</template>

<script>
export default {
  name: 'parallax',
  props: {
      title: String
  }
}
</script>