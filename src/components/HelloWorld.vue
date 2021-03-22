<template>
  <v-container fill-height>
    
    <!-- Jumbotron -->
    <v-row
        align="center"
        justify="center"
      >
        <h1 class="text-center display-3 hidden-xs-only">
          Bienvenue sur Echo'munication
        </h1>
        <span class="text-center subheading hidden-xs-only">Le site vise à répertorier des tutoriels sélectionnés pour et par les Développeurs Web en formation à Réalise.</span>

        <h1 class="text-center display-1 hidden-sm-and-up">
         Bienvenue sur Echo'munication
        </h1>
        <span class="text-center subheading hidden-sm-and-up">Le site vise à répertorier des tutoriels sélectionnés pour et par les Développeurs Web en formation à Réalise.</span>
      </v-row>

            
    <v-row>
      <!-- Section de recherche -->
      <v-col sm="5" offset="1">
        <v-card>
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
                  required
                ></v-text-field>

                <v-text-field
                    v-model="email"
                    label="avec le langage (PHP, JavaScript, CSS, ...)"
                    required
                ></v-text-field>

                  <v-btn
                    :disabled="!valid"
                    color="primary"
                    class="mr-4"
                    @click="validate"
                  >
                  <v-icon left>mdi-text-box-search-outline</v-icon>
                    Lancer la recherche
                  </v-btn>
                </v-form>
          </v-card-subtitle>
        </v-card>
      </v-col>


      <v-col sm="5">
        <v-card class="align-stretch">
            <v-card-title>Ajout de tutoriel</v-card-title>
            <v-card-subtitle>Vous avez regardé, écouté ou lu un tutoriel de qualité que vous souhaiteriez partager ?</v-card-subtitle>
              <v-card-actions>
                <v-btn>
                  <v-icon left>mdi-plus-circle</v-icon>
                  Proposer un tutoriel</v-btn>
              </v-card-actions>
        </v-card>
      </v-col>

    </v-row>
  </v-container>
</template>

<script>
  export default {
    name: 'HelloWorld'
  }
</script>
