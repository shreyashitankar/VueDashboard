<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/2.7.1/Chart.min.js"></script>
<script src="https://unpkg.com/vue-chartjs/dist/vue-chartjs.min.js"></script>

<template>
<div class="linechart">
    <v-row class="ml-1 title1"> 
        <v-card class="pa-3"  flat> 
         <v-list-item-title class="blue-grey--text title" >Traffic</v-list-item-title>
        <v-list-item-subtitle class="grey--text">May 2020</v-list-item-subtitle>
        </v-card>
        <v-spacer></v-spacer>
        <v-card class="text-center mr-3 mt-5" flat>
          
      <v-btn  tile outlined color="blue-grey lighten-1">Day</v-btn>
      <v-btn  tile color="blue-grey lighten-1" dark >Month</v-btn>
      <v-btn  tile outlined color="blue-grey lighten-1">Year</v-btn>
      <v-btn class="ml-2" icon color="indigo"><v-icon>mdi-cloud-download</v-icon></v-btn>
      
        </v-card>
        </v-row>
          <br />
          <area-chart :data="chartData" :colors="['#b4e4fa']"></area-chart> 
</div> 
</template>

<script>
export default {
    name:"Linechart",
     data(){
      return{
        chartData:{
          '2017-05-13': 2,
          '2017-05-14':5,
          "2017-05-15":4,
          "2017-05-16":1,
          "2017-05-17":9,
          "2017-05-18":6,
          
        }
      }
    },
}
</script>