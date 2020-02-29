<template>
    <v-card
            max-width="750"
            height="200"
            class="mx-auto"
            style="margin-right: 200px;"
    >

        <v-img
                src="https://www.sneakers-actus.fr/wp-content/uploads/2018/06/converse-one-star-golf-le-fleur-rouge-et-bleu-couv.jpg"
                height="550"
                width="1500"
        ></v-img>



        <v-card-actions>

            <v-spacer></v-spacer>
            <v-btn icon>
                <v-icon>mdi-heart</v-icon>
            </v-btn>

        </v-card-actions>
    </v-card>

</template>

<script>

    export default {

        props:{
            name: String,
            img: String,

            }


    }
</script>