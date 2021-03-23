<template>
    <v-col 
        sm="5"
    >
        <!-- La hauteur de 100% permet de faire en sorte que les deux cartes aient la même taille -->
          <v-card 
            class="align-stretch elevation-5" 
            height="100%" 
          > 
              <v-card-title>
                Ajout de tutoriel
              </v-card-title>
              <v-card-subtitle>
                Vous avez regardé, écouté ou lu un tutoriel de qualité que vous souhaiteriez partager ?
              </v-card-subtitle>
                <v-card-actions>
                  <v-btn color="primary">
                    <v-icon left>mdi-plus-circle</v-icon>
                    Proposer un tutoriel</v-btn>
                </v-card-actions>
          </v-card>
      </v-col>
</template>

<script>
export default {
    name: 'AddingTutorialCard'
}
</script>