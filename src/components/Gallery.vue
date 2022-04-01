<template>
    <v-row>
        <v-col>
        </v-col> 
    </v-row>
    <v-row>
        <v-col
        v-for="n in 8"
        :key="n"
        class="d-flex child-flex"
        cols="3"
        >
            <v-img
                :src="require(`../assets/mejalosa${n}.jpeg`)"
                :lazy-src="`https://picsum.photos/400/600`"
                aspect-ratio="1"
                class="grey lighten-2"
            >
                <template v-slot:placeholder>
                <v-row
                    class="fill-height ma-0"
                    align="center"
                    justify="center"
                >
                    <v-progress-circular
                    indeterminate
                    color="grey lighten-5"
                    ></v-progress-circular>
                </v-row>
                </template>
            </v-img>
        </v-col>
    </v-row>
</template>

<script>
export default {
  name: 'GalleryView',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
