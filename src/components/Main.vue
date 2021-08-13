<template>
    <v-container class="mt-16 mb-16">
          <v-row no-gutters>
            <v-col sm="4">
             <div>
              <v-img src="../assets/me.png"></v-img>
             </div>
            </v-col>
            <v-col sm="8" class="blue-grey lighten-5 pa-10">
              <h1 class="display-1 font-weight-thin text-center mb-12">{{title}}</h1>
              <h4>{{subtitle}}</h4>
              <br>
              <p>{{content}}</p>
            </v-col>
          </v-row>
        </v-container>
</template>

<script>
export default {
  name: 'mainContent',
  props: {
      title: String,
      subtitle: String,
      content: String
  }
}
</script>