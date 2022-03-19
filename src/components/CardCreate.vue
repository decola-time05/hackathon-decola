<template>
    <v-card
    class="mx-auto my-5"
    max-width="344"
  >
    <v-img
      :src=card.photo
      height="350px"
      width="350px"
    ></v-img>

    <v-card-title>
      {{card.name}}
    </v-card-title>

    <v-card-subtitle>
      {{card.address}}
    </v-card-subtitle>

    <v-card-actions>
      <v-btn
        color="amber darken-4"
        text
      >
        ASSISTA AO VIVO
      </v-btn>

      <v-spacer></v-spacer>

      <v-btn
        icon
        @click="show = !show"
      >
        <v-icon>{{ show ? 'mdi-chevron-up' : 'mdi-chevron-down' }}</v-icon>
      </v-btn>
    </v-card-actions>

    <v-expand-transition>
      <div v-show="show">
        <v-divider></v-divider>

        <v-card-text>
          {{card.description}}
        </v-card-text>
      </div>
    </v-expand-transition>
  </v-card>
</template>

<script>
export default {
    name:'CardCreate',
    props:['card'],
    data: () => ({
      show: false,
      
    }),
}
</script>

<style scoped>

</style>