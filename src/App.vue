<template>
   <v-app id="app">
      <v-navigation-drawer
      color="green"
      dark
      expand-on-hover
      hide-overlay
      permanent
      right
      app
      >
      <v-list
       nav 
      shaped
      dense
      >
      <v-list-item two-line>
       <v-list-item-avatar>
         <img src="https://randomuser.me/api/portraits/men/1.jpg" alt="">
      </v-list-item>
      <v-list-item-content class="text-left">
        <v-list-item-title class="font-weight-black">SocialLink</v-list-item-title>
        <v-list-item-subtitle>Иван Иванов</v-list-item-subtitle>
      </v-list-item-content>
      </v-list>
      </v-navigation-drawer>
    
    <v-content class="px-12 py-3">
      <v-container fluid>
        <router-view/>
      </v-container>
    </v-content>

  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld';

export default {
  name: 'App',

  components: {
    HelloWorld,
  },

  data: () => ({
    //
  }),
};
</script>
