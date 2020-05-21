<template>
    
    <v-navigation-drawer v-model="drawer" app  class="" >
      <v-list dense>
        <v-list-item @click.stop="left = !left">
          <v-list-item-action>
            <v-icon>mdi-exit-to-app</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Open Temporary Drawer</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    
</template>

<script>
export default {
    name:"Drawer"
}
</script>

<style scoped>
.v-navigation-drawer__content {
    height: 100%;
    overflow-y: auto;
    overflow-x: hidden;
    
}
</style>