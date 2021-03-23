<template>
    <v-row>
        <v-row class="mt-14">
            <v-col offset="">
                <h2 class="display-1 mb-4">Catégories à parcourir</h2>
            </v-col>
        </v-row>

      <v-row>
        <v-col
          xs="6"
          sm="6"
          md="4"
          lg="4"
          v-for="category in categories" :key="category.name"
        >
          <v-card hover class="mb-5">
            
            <v-row>
              <v-col cols="1" :style="{'background-color': category.color}">
              </v-col>
              <v-col>
                <v-card-title>{{ category.name }}</v-card-title>
 
              </v-col>
            </v-row>

          </v-card>
        </v-col>
      </v-row>
    </v-row>
</template>

<script>
export default {
    name: 'HomeCategories',
    data: function () {
      return {
        categories: [
          { 
            name: 'Algorithmie',
            color: 'lightgrey',
          },
          { 
            name: 'Bootstrap',
            color: '#6d10ed',
          },
          { 
            name: 'CSS',
            color: '#2c4de4',
          },
          { 
            name: 'Docker',
            link: '',
            color: '#2391e6',
          },
          { 
            name: 'Javascript',
            color: '#f7df2c',
          },
          { 
            name: 'Laravel',
            color: '#ff2927',
          },
          { 
            name: 'PHP',
            color: '#7377ad',
          },
          { 
            name: 'React',
            color: '#62dafb',
          },
          { 
            name: 'Vue',
            color: '#3fba84',
          },
        ]
      }
    }
}
</script>