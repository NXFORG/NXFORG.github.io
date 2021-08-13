<template>
    <v-carousel height="800">
         <v-carousel-item v-for="item in slides" :key="item" :src="item.img" reverse-transition="fade-transition" transition="fade-transition">
           <v-row class="align-end blue-grey lighten-5" justify="center" height="200">
             <v-col class="text-center mt-6" cols="12">
              <h1 class="black--text font-weight-thin">{{item.title}}</h1>
             </v-col>
             <v-col class="text-center" cols="12">
              <p class="black--text">{{item.label}}</p>
             </v-col>
            </v-row>
         </v-carousel-item>
        </v-carousel>
</template>


<script>
export default {
  name: 'carousel',
  data: () => ({
       slides: [
       {
         img: require("../assets/merc.jpeg"),
         title: "Where I'm From",
         label: "I grew up in the Brooklands area which is known for having the world's first purpose-built racetrack.",
       },
       {
         img: require("../assets/portsdown2.jpeg"),
         title: "Things I Enjoy",
         label: "I'm always looking for my next adventure, whether that's exploring nature or publicly accessible abandoned urban locations.",
       },
       {
         img: require("../assets/music.jpeg"),
         title: "Things I Enjoy",
         label: "A passionate audiophine, I always strive to get the best possible sound quality from my music.",
       },
       {
         img: require("../assets/flumserberg.jpeg"),
         title: "Places I've travelled",
         label:  "I've had the opportunity to visit many outstanding locations in the UK and abroad. One of the highlights of my travels is the Swiss Alps.",
       },
       ]
     })
}
</script>