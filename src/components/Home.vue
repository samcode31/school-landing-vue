<template>
  <v-container
    class="pa-0"
    fluid
  >
    <v-row class="text-center">
      <!-- <v-col cols="12">
        <v-img
          :src="require('../assets/logo.png')"
          class="my-3"
          contain
          height="200"
        />
      </v-col> -->

      <!-- <v-col class="mb-4">
        <h1 class="display-2 font-weight-bold mb-3">
          Welcome to EL Dorado East Secondary
        </h1>

        <p class="subheading font-weight-regular">
          For latest information on the school,
          <br>please join us online          
        </p>
      </v-col> -->

      <v-carousel>
        <v-carousel-item
          v-for="(item, i) in wallpapers"
          :key="i"
          :src="item.src"
          reverse-transition="fade-transition"
          transition="fade-transition"
          cycle
          continuous
        ></v-carousel-item>
      </v-carousel>
      <v-card
        class="mx-auto"
        flat
        width="800"
      >
        <v-card-text>
          <v-row
            align="center"
            justify="center"
            class="indigo--text font-weight-light text-h3"
            
          >
           
              <div>2020 FORM 1 REGISTRATION</div>
           
              
           
          </v-row>
          <v-row
            align="center"
            justify="center"
            class="mt-6"
          >
            <v-btn
                color="indigo"
                dark
                x-large
                class="ml-4 font-weight-thin"
                href="https://eldorado-east-student-registration.ttschoolnet.org"
              >
              Click Here To Register
              </v-btn>
          </v-row>
        </v-card-text>
        <v-card-actions>
          
        </v-card-actions>
      </v-card>

    </v-row>
  </v-container>
</template>

<script>
  export default {
    name: 'Home',

    data: () => ({
      wallpapers: [
        {src: require('../assets/wallpapers/wallpaper-1.jpg')},
        {src: require('../assets/wallpapers/wallpaper-2.jpg')},
        {src: require('../assets/wallpapers/wallpaper-3.jpg')},
      ]
    }),
  }
</script>
