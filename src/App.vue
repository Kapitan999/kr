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
    dense>
     <v-list-item two line>
     <v-list-item-avatar>
     
     </v-list-item-avatar>
     </v-list-item>
    </v-list>
    
      </v-navigation-drawer>
    
    <v-content class="px-12 py-3">
      <v-container fluid>
        <v-container/>
      </v-container>
    </v-content>

  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    v-app: () => import('./app.vue'),
    v-navigation-drawer: () => import('./app.vue'),
    v-list: () => import('./app.vue'),
    v-list-item: () => import('./app.vue'),
    v-list-item-avatar: () => import('./app.vue'),
    v-content: () => import('./app.vue'),
    v-container: () => import('./app.vue'),
    v-container: () => import('./app.vue')
  }
}
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
