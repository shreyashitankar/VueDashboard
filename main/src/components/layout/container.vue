<template>
    <v-app class="Container" >
        <v-container
        class="fill-height"
        fluid
        
      >
      <Grid/>
      </v-container>
    </v-app>
</template>
<script>
import Grid from './containergrids'

export default {
    name:"Container",
    components:{
        Grid
    }
}
</script>