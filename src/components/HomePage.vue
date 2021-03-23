<template>
  <v-container fill-height>
    
    <!-- Hero -->
    <HomeHero />

    <!-- Deux cartes de recherche et ajout de tutos -->   
    <v-row>
      <SearchingTutorialCard />
      <AddingTutorialCard />
    </v-row>

    <!-- Sidebar -->

    <!-- Boucle de cartes des catégories -->
    <HomeCategories />

  </v-container>
</template>

<script>
  import HomeHero from '../pages/HomePage/HomeHero'
  import SearchingTutorialCard from '../pages/HomePage/SearchingTutorialCard'
  import AddingTutorialCard from '../pages/HomePage/AddingTutorialCard'
  import HomeCategories from '../pages/HomePage/HomeCategories'

  export default {
    name: 'HomePage',
    components: {
      HomeHero,
      SearchingTutorialCard,
      AddingTutorialCard,
      HomeCategories
    },
  }
</script>
