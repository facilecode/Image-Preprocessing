<template>
  <div class="conv">
    
    <v-row align="center" justify="center">
        <v-col >
            <v-card class="mx-auto" max-width="400" >
                <v-img src="../assets/mustang.jpg" width="400" height="400" ></v-img>

                <v-card-title>
                    Title
                </v-card-title>
                <v-card-subtitle>
                    Subtitle
                </v-card-subtitle>

                <v-card-actions>
                <v-btn color="orange lighten-2" text > Explore </v-btn>
                <v-spacer></v-spacer>
                <v-btn color="orange lighten-2" text >Load Image</v-btn>
                </v-card-actions>
            </v-card>  
        </v-col>
        <!-- filter -->
        <v-col>
            <v-container>
                <v-row>
                    <v-col v-for="(n,index) in filter_array" :key="index" :cols="n_cols">
                        <v-card width="40px" height="40px">
                            <v-text-field :label="filter_array[index]"></v-text-field>
                        </v-card>
                    </v-col>
                    <v-col>
                        <v-btn>right</v-btn>
                    </v-col>
                </v-row>
                <v-row>
                    <v-btn height="50px" width="400px">down</v-btn>
                </v-row>
            </v-container>
        </v-col>
        <!-- end-filter -->
        <v-col>
            <v-card class="mx-auto" max-width="400" >
                <v-img src="../assets/mustang.jpg" width="400" height="400" ></v-img>

                <v-card-title>
                    Title
                </v-card-title>
                <v-card-subtitle>
                    Subtitle
                </v-card-subtitle>

                <v-card-actions>
                <v-btn color="orange lighten-2" text > Explore </v-btn>
                <v-spacer></v-spacer>
                <v-btn color="orange lighten-2" text >Load Image</v-btn>
                </v-card-actions>
            </v-card>  
        </v-col>
    </v-row>
 

  </div>
</template>

<script>
//import * as tf from '@tensorflow/tfjs'

export default {
  name: 'Conv',

  data(){
      return {
          model: null,
          show: true,
          filter_array: [1,2,3,4,5,6,7,8,9],
          n_rows: 3,
          n_cols: 4
      }
  },
  mounted() {
    
  }
}
</script>

<style scoped>

</style>
