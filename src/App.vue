<template>
  <v-app>
    <NavBar />
    <v-main>
      <router-view />
    </v-main>
    <app-footer/>
  </v-app>
</template>

<script>
import NavBar from "./components/shared/NavBar.vue";
import AppFooter from '@/components/shared/AppFooter.vue'

export default {
  name: "App",

  components: {
    NavBar,
    AppFooter,
  },
};
</script>

<style scoped>
</style>