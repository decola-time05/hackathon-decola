<template>
  <v-app>
   <NavBar/>
    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script>

import NavBar from './components/shared/NavBar.vue'

export default {
  name: "App",

  components: {
    NavBar,
  },
};
</script>

<style scoped>
</style>