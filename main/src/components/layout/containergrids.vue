<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/2.7.1/Chart.min.js"></script>
<script src="https://unpkg.com/vue-chartjs/dist/vue-chartjs.min.js"></script>

<template>
    <v-app class="grid" id="inspire" >
      
     <v-container class="grey lighten-5" fluid width="100%" >
    <v-row no-gutters>
      <v-col
      cols="12">
      <Gridheader/>
      </v-col>
      <v-col
        cols="12"
      >
        <v-card
          class="box pa-2"
          outlined
          
        >
        <Linechart/>

        <v-divider></v-divider>
        <Stats/>  
        </v-card>
      </v-col>
      
    </v-row>
  </v-container>
    </v-app>
</template>
<script>
import Stats from "../layout/statsgrid1"
import Linechart from "../layout/linechart"
import Gridheader from "../layout/GridHead"
export default {
    name:"Grid",
    components:{
      Stats,
      Linechart,
      Gridheader
    }
}

</script>




<style scoped>
.grid{
  width: 100%;
}

</style>