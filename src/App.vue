<template>
  <v-app>
    <v-app-bar
      app
      color="indigo"
      dark
    >
      <div class="d-flex align-center">
        <v-img
          alt="school Logo"
          class="shrink mr-2"
          contain
          :src="require('./assets/logo.png')"
          transition="scale-transition"
          width="40"
        />

        
      </div>
      <div class="text-uppercase">El Dorado East Secondary School</div>

      <v-spacer></v-spacer>

      
    </v-app-bar>

    <v-main>
      <Home/>
    </v-main>
    <v-footer
      dark
      padless
    >
      <v-card
        flat
        tile
        class="indigo white--text text-center"
        width="100%"
      >
        <v-card-text>
          <v-btn 
            class="mx-4 white--text font-weight-light"
            text
          >
            <v-icon left>mdi-phone</v-icon>
            +1 868 662 2608 | +1 868 662 8605
          </v-btn>
          <v-btn 
            class="mx-4 white--text font-weight-light"
            text
          >
            <v-icon left>mdi-email</v-icon>
            eldoradoeast.sec@fac.edu.tt
          </v-btn>
          <v-btn 
            class="mx-4 white--text font-weight-light"
            text
          >
            <v-icon left>mdi-office-building-marker-outline</v-icon>
            1 Karamath Street El Dorado
          </v-btn>
        </v-card-text>
        
      </v-card>
    </v-footer>
  </v-app>
</template>

<script>
import Home from './components/Home';

export default {
  name: 'App',

  components: {
    Home,
  },

  data: () => ({
    //
  }),
};
</script>
