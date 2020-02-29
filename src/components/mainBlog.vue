<template>
  <v-card
          class="mx-center"
          color="#00000"
          dark
          max-width="290"

          style="margin-left: 1100px;
                margin-bottom: 40px"

  >
    <v-card-title>

    </v-card-title>

    <v-card-text class="headline font-weight-bold">
      "Just Do It."
    </v-card-text>

    <v-card-actions>
      <v-list-item class="grow">
        <v-list-item-avatar color="grey darken-3">
          <v-img
                  class="elevation-6"
                  src="https://www.episod.com/wp-content/uploads/2019/04/b2b-logo-nike.jpg"
          ></v-img>
        </v-list-item-avatar>

        <v-list-item-content>
          <v-list-item-title>Nike</v-list-item-title>
        </v-list-item-content>


      </v-list-item>
    </v-card-actions>
  </v-card>

</template>

<script>
  export default {
    name: 'mainBlog',
      props:{
      name:String,
      description:String,
      img:String,
      }
    }
</script>


