<template>
<v-card
    elevation="24"
    max-width="444"
    class="mx-auto"
  >
    <v-system-bar lights-out></v-system-bar>
    <v-carousel
      :continuous="false"
      :cycle="cycle"
      :show-arrows="false"
      hide-delimiter-background
      delimiter-icon="mdi-minus"
      height="300"
    >
      <v-carousel-item
        v-for="(item, i) in items"
        :key="i"
        :src="item.src"
      >
       
          <v-row
            class="fill-height"
            align="center"
            justify="center"
          >
          </v-row>
        
      </v-carousel-item>
    </v-carousel>
    <v-list two-line>
      <v-list-item>
        <v-list-item-avatar>
          <v-img src="https://cdn.vuetifyjs.com/images/john.png"></v-img>
        </v-list-item-avatar>
        <v-list-item-content>
          <v-list-item-title>John Leider</v-list-item-title>
          <v-list-item-subtitle>Author</v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>
    </v-list>
  </v-card>
</template>

<script>
  export default {
    data () {
      return {
        cycle: true,
        items: [
          {
            src: require('../assets/carnaval01.jpg'),
          },
          {
            src: require('../assets/carnaval02.jpg'),
          },
          {
            src: require('../assets/carnaval03.jpg'),
          },
          {
            src: require('../assets/carnaval04.jpg'),
          },
        ],
      }
    },
  }
</script>