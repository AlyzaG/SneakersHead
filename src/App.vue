<template>
  <v-app>

    <v-app-bar
      app
      color="black"
      dark
      style="height: 70px"
    >
        <h1>SneakersHead</h1>
    </v-app-bar>

    <v-spacer></v-spacer>


    <v-content>

      <v-carousel hide-delimiters height="730px">
        <v-carousel-item
                v-for="(item,i) in items"
                :key="i"
                :src="item.src"
        ></v-carousel-item>
      </v-carousel>
      <v-spacer></v-spacer>
      <h1 class="text-center" style="margin: 40px"> La Sneakers du mois </h1>

      <div class="container">
        <div class="row" style="margin-right: 190px;">
          <articles>
          </articles>
        </div>
      </div>

      <div>
        <main-blog/>
      </div>

    <div class="container" style=" margin-top: 320px" >
      <div class="row">
        <insta-posts username="Size?" image="https://i.pinimg.com/564x/9a/94/3f/9a943f12f73b029b8bb7f2330eae573f.jpg"></insta-posts>
        <insta-posts username="Size?"></insta-posts>
        <insta-posts username="Size?"></insta-posts>
      </div>

    </div>


    </v-content>


  </v-app>
</template>

<script>

import mainBlog from './components/mainBlog';
import articles from "./components/articles";
import instaPosts from "./components/instaPosts";

export default {
  name: 'App',

  components: {
    mainBlog,
    articles,
    instaPosts,

  },
  data () {
    return {
      items: [
        {
          src: 'https://image-cdn.hypb.st/https%3A%2F%2Fhypebeast.com%2Fwp-content%2Fblogs.dir%2F11%2Ffiles%2F2019%2F11%2Fblack-friday-sneakers-mode-vetements-soldes-promos-offres-liste-1.jpg?q=75&w=800&cbr=1&fit=max',
        },
        {
          src: 'https://www.lesbroussettes.fr/wp-content/uploads/2019/03/Sneaker-Nike-Air-Max-1024x683.jpg',
        },
        {
          src: 'https://media.vogue.fr/photos/5d40515bc93b83000833392f/16:9/w_1920,c_limit/020-Sneakers-Encyclopaedia-Vogueint-Jul24-Getty-Images.jpg',
        },
        {
          src: 'https://www.sneakerdistrict.de/images2/Puma-RS-X-Colour-Theory-Whisper-White-Puma-Black-2-800.jpg',
        },
      ],
    }

  },
}



</script>
