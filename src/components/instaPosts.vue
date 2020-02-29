<template>
    <v-card
            max-width="344"
            class="mx-auto"
    >
        <v-list-item>
            <v-img src="logosize.png" height="" width=""></v-img>
            <v-list-item-content>
                <v-list-item-title class="headline">{{username}}</v-list-item-title>

            </v-list-item-content>
        </v-list-item>

        <v-img
                src=""

                height="194"
        ></v-img>

        <v-card-text>
            Visit ten places on our planet that are undergoing the biggest changes today.
        </v-card-text>


    </v-card>
</template>

<script>

    export default {
        props:{
            username: String,
            image: String,
            comments: String,
            profilimg: String

        }
    }
</script>