<template>
  <v-app>
    <v-app-bar
      app
      color="primary"
      dark
    >
      <v-toolbar-title>Echo'Munication</v-toolbar-title>
      <v-spacer></v-spacer>
      
      <!-- Doivent rapidement être remplacés par une boucle -->
      <v-btn
        href="#"
        text
      >
        <span class="mr-2">Accueil</span>
      </v-btn>

      <v-btn
        href="#"
        text
      >
        <span class="mr-2">Tutoriels</span>
      </v-btn>

      <v-btn
        href="#"
        text
      >
        <span class="mr-2">Mes favoris</span>
      </v-btn>

      <v-btn
        href="#"
        text
      >
        <span class="mr-2">Se connecter</span>
      </v-btn>

        <!-- <v-icon>mdi-open-in-new</v-icon> -->
    </v-app-bar>

    <v-main>
      <HelloWorld/>
    </v-main>

  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld';

export default {
  name: 'App',

  components: {
    HelloWorld,
  },

  data: () => ({
    //
  }),
};
</script>
