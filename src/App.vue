<template>
   <v-app>
      <v-navigation-drawer v-model="drawer"
         app
         clipped>
      </v-navigation-drawer>

      <v-content>
         <HomeComponent/>
      </v-content>
   </v-app>
</template>

<script>
import HomeComponent from './components/HomeComponent';

export default {
   name: 'App',
   components: {
      HomeComponent,
   },
   data: () => ({
      drawer: null,
   }),
   created () {
      this.$vuetify.theme.dark = true
   },
};
</script>
