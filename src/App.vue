<template>
  <v-app>
    <v-main>
        <v-parallax
          dark
          src="./assets/banner.jpeg"
          height=250px
        >
        <Header />
        </v-parallax>
       
       <Gallery/>
       <Footer/>
    </v-main>    
  </v-app>
</template>

<script>
  import Header from './components/Header.vue'
  import Gallery from './components/Gallery.vue'
  import Footer from './components/Footer.vue'
  export default {
    name: 'App',

    components: {
      Header,
      Gallery,
      Footer
    },

    data: () => ({
      drawer: false,
      group: null,
    }),
  }
</script>
