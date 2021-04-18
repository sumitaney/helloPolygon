<template>
<nav>
  <v-app-bar flat app class="transparent">
    
      <v-spacer></v-spacer>
     
     <div class="">
              <v-menu offset-y  bottom
            left>
      <template v-slot:activator="{ on, attrs }">
        <v-btn
          v-bind="attrs"
          v-on="on"
          elevation="0"
          tile
          icon
          class="transparent"
        >
          <i class="fa fa-2x grey--text darken-3 fa-bullhorn"></i>
        </v-btn>
      </template>
      <v-list class="grey darken-3 white--text px-5">
      
          <v-list-item-title class="mb-1"><v-icon color="light-blue darken-3">mdi-twitter</v-icon> Twitter</v-list-item-title>
          <v-list-item-title class="mb-1"><v-icon color="deep-orange darken-1">mdi-reddit</v-icon> Reddit</v-list-item-title>
          <v-list-item-title class="mb-1"><v-icon color="deep-purple darken-1">mdi-blogger</v-icon> Blog</v-list-item-title>
          <v-list-item-title class="mb-1"><v-icon color="amber darken-1">mdi-email-newsletter</v-icon> Newsletter</v-list-item-title>
      
      </v-list>
    </v-menu>
      
      <v-app-bar-nav-icon color="white" icon x-large class="grey--text px-2" tile @click="drawer = !drawer"></v-app-bar-nav-icon>
     </div>
    </v-app-bar>
    <v-navigation-drawer app temporary
     right v-model="drawer" class="grey darken-4 text-center" width="300">
     <div class="d-flex flex-column">
         <v-btn elevation="0" href="#top" class="text-h5 text-md-h5 transparent white--text mx-auto my-10 py-10">Home</v-btn>
       <v-btn elevation="0"   href="#mid" class="text-h6 text-md-h5 transparent white--text mx-auto mb-10 py-10">Services</v-btn>
       <v-btn elevation="0"   href="#mid"  class="text-h6 text-md-h5  transparent white--text mx-auto mb-10 py-10">Who's it for</v-btn>
       <v-btn elevation="0"   href="#bottom" class="text-h6 text-md-h5 transparent white--text mx-auto mb-10 py-10">About Us</v-btn>
      
           <v-btn color="grey" class="px-5 mx-5" bottom elevation="1" x-large>Sign in</v-btn>
      
       
     </div>
       
    </v-navigation-drawer>
</nav>
  
</template>

<script>
export default {
       name: 'Navbar',
data() {
    return {
        drawer: false,
    }
},
}
</script>

<style>

</style>