<template>
      <div>
    <v-row class="justify-center">
        <CardCreate v-for="(card,index) in blocosLista" :key="index" :card="card"/>
    </v-row>
  </div>
</template>
<script>
import CardCreate from "./CardCreate.vue";
export default {
    components: {
    CardCreate,
  },
  data() {
    return {
        blocosLista: [],
    };
  },
  async created() {
    const response = await fetch(
      "https://it3-hbn-default-rtdb.firebaseio.com/carnaval.json"
    );
    const converted = await response.json();
    this.blocosLista = converted.reverse();
  },
}
</script>
<style scoped>

</style>