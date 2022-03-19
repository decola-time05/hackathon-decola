<template>
  <v-app>
   <NavBar/>
   <HelloWorld/>
   </v-app>
</template>

<script>

import NavBar from './components/shared/NavBar.vue'
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: "App",

    components: {
    NavBar,
    HelloWorld,
  },
};
</script>

<style scoped>
</style>