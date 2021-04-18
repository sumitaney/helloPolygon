<template>
  <v-app>

 <Navbar/>
    <v-main>
      <HomePage/>
    </v-main>
  </v-app>
</template>

<script>
import HomePage from './components/HomePage';
import Navbar from './components/Navbar';

export default {
  name: 'App',

  components: {
    HomePage,
    Navbar
  },

  data: () => ({
    //
  }),
};
</script>

<style >

</style>