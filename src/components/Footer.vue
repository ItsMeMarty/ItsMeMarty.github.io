<template>
  <v-footer
    dark
    padless
  >
    <v-col
      class="text-center"
      cols="12"
    >
    
    <v-card
      flat
      tile
      
      class="indigo lighten-1 white--text text-center"
    >
      <v-card-text>
        <v-btn
          class="mx-4 white--text"
          href="https://www.instagram.com/mejalosa/"
        >
          <v-icon size="24px">
            mdi-instagram
          </v-icon>
        </v-btn>
      </v-card-text>

      <v-divider></v-divider>

      <v-card-text class="white--text">
        Copyright © {{ new Date().getFullYear() }} <strong>Mejalosa</strong>. All Rights Reserved 
      </v-card-text>
    </v-card>
    </v-col>
  </v-footer>
</template>

<script>
export default {
  name: 'FooterView',
  data: () => ({
      icons: [
        'mdi-facebook',
        'mdi-twitter',
        'mdi-linkedin',
        'mdi-instagram',
      ],
    }),
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
