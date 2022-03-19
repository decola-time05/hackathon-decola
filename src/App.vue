<template>
  <v-app>
   <NavBar/>
  </v-app>
</template>

<script>

import NavBar from './components/shared/NavBar.vue'

export default {
  name: 'App',

    components: {
    NavBar,
  },
};
</script>
