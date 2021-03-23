<template>
  <v-app>
    <AppHeader />

    <v-main>
      <HomePage />
    </v-main>

    <AppFooter />
  </v-app>
</template>

<script>
import HomePage from './components/HomePage';
import AppHeader from './components/layout/AppHeader';
import AppFooter from './components/layout/AppFooter';

export default {
  name: 'App',

  components: {
    HomePage,
    AppHeader,
    AppFooter,
  },

  data: () => ({
    //
  }),
};
</script>
