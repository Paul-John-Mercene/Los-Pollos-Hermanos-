<template>
  <v-app>
    <v-app-bar
      color="#379683"
      app
      flat
    >
    <Header/>
    </v-app-bar>
    
    <router-view></router-view>

    <v-footer>
      <Footer/>
    </v-footer>
  </v-app>
</template>

<script>
import Header from './components/Header';
import Footer from './components/Footer';

export default {
  name: 'App',

  components: {
    Header,
    Footer
  },

  data: () => ({
    //
  }),
};
</script>
