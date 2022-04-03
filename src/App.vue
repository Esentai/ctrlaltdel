<template>
  <v-app>
   

   <Menu/>
    <v-main>
   
    <Navigation/>    
    <v-container fluid>
      <router-view>
        <Cyberbullying v-if="currentPage == 'cyberbullying'" />
        <Map  v-if="currentPage == 'map'" />
      </router-view>
    </v-container>
   
    </v-main>

  </v-app>
</template>

<script>
import Menu from './components/Menu.vue';
import Navigation from './components/Navigation.vue';
import Cyberbullying from './components/Cyberbullying.vue';
import Map from './components/Map.vue';

export default {
  name: 'App',
  components:{
    Navigation,
    Menu,
    Cyberbullying,
    Map
  },
  data: () => {
      return ({
          currentPage:'map'
      })
  },
};
</script>
