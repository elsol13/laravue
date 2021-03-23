<template>
    <v-col sm="5" offset="1">
        <v-card 
          class="elevation-5"
          height="100%" 
        >
            <v-card-title>Recherche de tutoriels</v-card-title>
              <v-card-subtitle>
              <v-form
                ref="form"
                v-model="valid"
                lazy-validation
              >
                <v-text-field
                  v-model="name"
                  label="Je veux apprendre à (faire des formulaires, utiliser Flexbox, ...)"
                ></v-text-field>

                <v-text-field
                    v-model="email"
                    label="avec le langage (PHP, JavaScript, CSS, ...)"
                ></v-text-field>

                  <v-form-actions>
                    <v-btn color="primary">
                    <v-icon left>mdi-text-box-search-outline</v-icon>
                      Lancer la recherche
                    </v-btn>
                  </v-form-actions>

                </v-form>
          </v-card-subtitle>
        </v-card>
      </v-col>   
</template>

<script>
export default {
    name: 'SearchingTutorialCard'
}
</script>