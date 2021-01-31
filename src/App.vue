<template>
   <v-app id="app"
   color="grey">
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
      <v-list-item  two-line>
       <v-list-item-avatar>
         <img src="https://randomuser.me/api/portraits/men/1.jpg" alt="">
       </v-list-item-avatar>
      <v-list-item-content class="text-left">
        <v-list-item-title class="font-weight-black">SocialLink</v-list-item-title>
        <v-list-item-subtitle>Иван Иванов</v-list-item-subtitle>
      </v-list-item-content>
      </v-list-item>
      </v-list>
      <v-divider class="my-3"></v-divider>
      <v-list-item link :to="путь">
      <v-list-item-icon>
        <v-icon>mdi-home-outline</v-icon>
      </v-list-item-icon>
      <v-list-item-content class="text-left">
        <v-list-item-title class="text-left">Главная</v-list-item-title>
      </v-list-item-content>
      </v-list-item> 
      <v-list-item link :to="путь">
      <v-list-item-icon>
        <v-icon>mdi-account</v-icon>
      </v-list-item-icon>
      <v-list-item-content class="text-left">
        <v-list-item-title class="text-left">Мой профиль</v-list-item-title>
      </v-list-item-content>
      </v-list-item> 
      <v-list-item link :to="путь">
      <v-list-item-icon>
        <v-icon>mdi-account-multiple-plus</v-icon>
      </v-list-item-icon>
      <v-list-item-content class="text-left">
        <v-list-item-title class="text-left">Найти друзей</v-list-item-title>
      </v-list-item-content>
      </v-list-item>  
      </v-navigation-drawer>
    
    <v-content class="px-12 py-3">
      <v-container fluid>
        <router-view/>
      </v-container>
      <h1>SocialLink</h1>
      <h3>Новый формат делового общения</h3>
      <v-container two-line>
        <img src="https://st.depositphotos.com/1177973/3222/i/950/depositphotos_32221247-stock-photo-office-supplies-with-documents-and.jpg" alt="">
      </v-container>
    </v-content>

  </v-app>
</template>

<script>
//import HelloWorld from './components/HelloWorld';

export default {
  name: 'App',

  components: {
   // HelloWorld,
  },

  data: () => ({
    //
  }),
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
