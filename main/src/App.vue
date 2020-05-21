<template>
 <v-app id="inspire">
   
    <v-app-bar app clipped-right color="white" flat>
      <v-app-bar-nav-icon color="rgb(201, 199, 199)" @click.stop="drawer = !drawer">
      </v-app-bar-nav-icon>
      <v-card class="d-flex flex-row mb-6" color="transparent" flat tile>
        <Menu/>
        
      </v-card>
      
    </v-app-bar>

    <v-navigation-drawer  v-model="drawer" app color="rgb(48, 61, 84)">
      <v-list dense>
        <v-list-item @click.stop="left = !left">
          <v-list-item-action>
            <v-icon class="white--text">mdi-exit-to-app</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title class="white--text">Open Temporary Drawer</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
  
    
    
    <v-content >
      
     <Nav/>
      <Container />
    </v-content>

    <v-footer
      app
      color="blue-grey"
      class="white--text"
    >
      <span>Vuetify</span>
      <v-spacer></v-spacer>
      <span>&copy; 2019</span>
    </v-footer>
  </v-app>
</template>

<script>

import Menu from './components/menuitem'
import Nav from './components/appbar2'
import Container from './components/layout/container'
export default {
    components:{
      Menu,
      Nav,
      Container
    },
    props: {
      source: String,
    },
    data: () => ({
      drawer: null,
      drawerRight: null,
      right: false,
      left: false,
    })
  }</script>