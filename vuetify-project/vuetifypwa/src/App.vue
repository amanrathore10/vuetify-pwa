<template>
  <v-app>
    <v-navigation-drawer v-model="drawer" fixed clipped app>
  <v-list>
  <v-list-tile>Profile</v-list-tile>
  </v-list>
  </v-navigation-drawer>
  
  <v-toolbar color="purple"  app clipped-left >
  <v-toolbar-side-icon @click.native.stop="shownav" class="hidden-sm-and-up"> </v-toolbar-side-icon>
  <v-toolbar-title color="white" >Nozzberry</v-toolbar-title>  
 
  <v-spacer></v-spacer>
  <v-toolbar-items class="hidden-sm-and-down">

  <v-btn flat color="white">
  <v-icon left>account_circle</v-icon>
  Login</v-btn>
  <v-btn flat color="white">Signup</v-btn>
  <v-btn flat color="white">Profile</v-btn>
  </v-toolbar-items>
  
 
  </v-toolbar> 
  
  <main>
    <v-container fluid>
      <v-content>
        <router-view></router-view>
      </v-content>
    </v-container>
  </main>
    
  </v-app>
</template>

<script>
import signup from './components/signup'
export default {
  components:{
    'signup':signup
  },
  data () {
    return {
      // clipped: false,
      drawer: false,
      // fixed: false,
      // items: [{
      //   icon: 'bubble_chart',
      //   title: 'Inspire'
      // }],
      // miniVariant: false,
      // right: true,
      // rightDrawer: false,
      title: 'Vuetify.js'
    }
  },
  methods:{
    shownav:function(){
      this.drawer = !this.drawer;
    }
  },
  name: 'App'
}
</script>
