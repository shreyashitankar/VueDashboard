<template>
 <v-container class="grey lighten-5 stats">
      <v-row no-gutters>
           <v-col
          cols="12"
          sm="1"
          class="margin"
        >
          <v-card
            class="pa-2 text-center"
           flat
            tile
          >
            
          </v-card>
        </v-col>
        <v-col
          cols="12"
          sm="2"
          class="margin"
        >
          <v-card
            class="pa-2 text-center"
            flat
            tile

          >
            <v-list-item two-line>
                <v-list-item-content>
                  <v-list-item-title>Visits</v-list-item-title>
                  <v-list-item-subtitle>29,032 users (40%)</v-list-item-subtitle>
                </v-list-item-content>
              </v-list-item>
            <v-progress-linear value="40" color="green"></v-progress-linear>
          </v-card>
        </v-col>
        <v-col
          cols="12"
          sm="2"
          class="margin"
        >
          <v-card
            class="pa-2 text-center"
            flat
            tile
          >
            <v-list-item two-line>
                <v-list-item-content>
                  <v-list-item-title>Unique</v-list-item-title>
                  <v-list-item-subtitle>24.094 users (20%)</v-list-item-subtitle>
                </v-list-item-content>
              </v-list-item>
            <v-progress-linear value="20" color="blue"></v-progress-linear>
          </v-card>
        </v-col>
        <v-col
          cols="12"
          sm="2"
          class="margin"
        >
          <v-card
            class="pa-2 text-center"
            flat
            tile
          >
            <v-list-item two-line>
                <v-list-item-content>
                  <v-list-item-title>Page Views</v-list-item-title>
                  <v-list-item-subtitle>78.706 views (60%)</v-list-item-subtitle>
                </v-list-item-content>
              </v-list-item>
            <v-progress-linear value="60" color="orange"></v-progress-linear>
          </v-card>
        </v-col>
        <v-col
          cols="12"
          sm="2"
          class="margin"
        >
          <v-card
            class="pa-2 text-center"
           flat
            tile
          >
            <v-list-item two-line>
                <v-list-item-content>
                  <v-list-item-title>New Users</v-list-item-title>
                  <v-list-item-subtitle>22.123 users (80%)</v-list-item-subtitle>
                </v-list-item-content>
              </v-list-item>
            <v-progress-linear value="60" color="red"></v-progress-linear>
          </v-card>
        </v-col>
        <v-col
          cols="12"
          sm="2"
          class="margin"
        >
          <v-card
            class="pa-2 text-center"
           flat
            tile
          >
            <v-list-item two-line>
                <v-list-item-content>
                  <v-list-item-title>Bounce Rate</v-list-item-title>
                  <v-list-item-subtitle>Average Rate (40.15%)</v-list-item-subtitle>
                </v-list-item-content>
              </v-list-item>
            <v-progress-linear value="40" color="indigo"></v-progress-linear>
          </v-card>
        </v-col>
         <v-col
          cols="12"
          sm="1"
          class="margin"
        >
          <v-card
            class="pa-2 text-center"
           flat
            tile
          >
            
          </v-card>
        </v-col>
      </v-row>
    </v-container>
</template>

<script>
export default {
    name:"Stats"
}
</script>

<style  scoped>
/* @media only screen and (max-width: 786px) {
    .margin{
        margin-left: 0;

}

}
.margin{
    margin-left:20px ;
} */

</style>