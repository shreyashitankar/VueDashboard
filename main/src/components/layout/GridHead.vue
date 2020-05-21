<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/2.7.1/Chart.min.js"></script>
<script src="https://unpkg.com/vue-chartjs/dist/vue-chartjs.min.js"></script>


<template>
    <v-container class="grey lighten-5 Gridhead">
      <!-- Stack the columns on mobile by making one full-width and the other half-width -->
      <!-- Columns start at 50% wide on mobile and bump up to 33.3% wide on desktop -->
      <v-row>
        <v-col
          cols="6"
          md="3"
          
        >
          <v-card
            class="pa-2"
            outlined
            tile
            color="blue lighten-2"
            
          >
         <v-card class="pa-3"  flat color="transparent"> 
        <v-btn class="ml-2 float-right" icon color="white"><v-icon>mdi-cloud-download</v-icon></v-btn>
          <v-list-item-title class="white--text title" >9823</v-list-item-title>
          <v-list-item-subtitle class="white--text">Members Online</v-list-item-subtitle>
          
        </v-card>
            <line-chart height="120px" :colors="['#fff']"  :library="chartOptions" :data="{'2017-05-13': 2, '2017-05-14': 5,  '2017-05-15': 3,  '2017-05-16': 4, '2017-05-16': 5,  '2017-05-17': 4}"></line-chart>
          </v-card>
        </v-col>
        <v-col
          cols="6"
          md="3"
          
        >
          <v-card
            class="pa-2"
            outlined
            tile
            color="indigo lighten-2"
            
          >
         <v-card class="pa-3"  flat color="transparent"> 
        <v-btn class="ml-2 float-right" icon color="white"><v-icon>mdi-cloud-download</v-icon></v-btn>
          <v-list-item-title class="white--text title" >9823</v-list-item-title>
          <v-list-item-subtitle class="white--text">Members Online</v-list-item-subtitle>
          
        </v-card>
            <line-chart height="120px" :curve="false" :colors="['#fff']"  :library="chartOptions" :data="{'2017-05-13': 2, '2017-05-14': 4,  '2017-05-15': 2,  '2017-05-16': 6, '2017-05-17': 2,  '2017-05-18': 3}"></line-chart>
          </v-card>
        </v-col>
        <v-col
          cols="6"
          md="3"
          
        >
          <v-card
            class="pa-2"
            outlined
            tile
            color="orange lighten-2"
            
          >
         <v-card class="pa-3"  flat color="transparent"> 
        <v-btn class="ml-2 float-right" icon color="white"><v-icon>mdi-cloud-download</v-icon></v-btn>
          <v-list-item-title class="white--text title" >9823</v-list-item-title>
          <v-list-item-subtitle class="white--text">Members Online</v-list-item-subtitle>
          
        </v-card>
            <column-chart height="120px" :colors="['#fff']" :library="chartOptions" :data="{'2017-05-13': 2, '2017-05-14': 5,  '2017-05-15': 3,  '2017-05-16': 4, '2017-05-17': 5,  '2017-05-18': 4}"></column-chart>
          </v-card>
        </v-col>
        <v-col
          cols="6"
          md="3"
          
        >
          <v-card
            class="pa-2"
            outlined
            tile
            color="red lighten-2"
            
          >
         <v-card class="pa-3"  flat color="transparent"> 
        <v-btn class="ml-2 float-right" icon color="white"><v-icon>mdi-cloud-download</v-icon></v-btn>
          <v-list-item-title class="white--text title" >9823</v-list-item-title>
          <v-list-item-subtitle class="white--text">Members Online</v-list-item-subtitle>
          
        </v-card>
            <area-chart :points="false" height="120px" :colors="['#fff']" :library="chartOptions" :data="{'2017-05-13': 2, '2017-05-14': 5,  '2017-05-15': 3,  '2017-05-16': 4, '2017-05-17': 5,  '2017-05-18': 4}"></area-chart>
          </v-card>
        </v-col>
      </v-row>
  
      <!-- Columns are always 50% wide, on mobile and desktop -->
      
    </v-container>
</template>

<script>
export default {
    name:"Gridhead",
    data(){
        return{
            chartOptions:{
                 layout: {
        padding: {left: 10, right: 5, top: 5, bottom: 2}
      },
      scales: {
        xAxes: [{
          display: false // this hides the x-axis
        }],
        yAxes: [{
          display: false // this hides the x-axis
        }]
      }}
        }
    }
}
</script>
<style  scoped>
.card1{
    background-color: rgb(0, 0, 0);
}
</style>