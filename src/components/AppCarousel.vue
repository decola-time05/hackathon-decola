<template>
  <v-card elevation="24" max-width="550" class="mx-auto my-6">
    <v-carousel
      :continuous="true"
      :cycle="true"
      :show-arrows="true"
      hide-delimiter-background
      delimiter-icon="mdi-minus"
      height="350"
    >
      <v-carousel-item v-for="(item, i) in items" :key="i" :src="item.src">
        <v-row class="fill-height" align="center" justify="center"> </v-row>
      </v-carousel-item>
    </v-carousel>
    <v-list two-line>
      <v-list-item>
        <v-list-item-avatar>
          <v-img src="../assets/instagram.png"></v-img>
        </v-list-item-avatar>
        <v-list-item-content>
          <a
            class="instagram"
            href="https://www.instagram.com/explore/tags/carnavalemcasa/"
            target="_blank"
            >@carnavalemcasa</a
          >
        </v-list-item-content>
      </v-list-item>
    </v-list>
  </v-card>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          src: require("../assets/carnaval01.jpg"),
        },
        {
          src: require("../assets/carnaval02.jpg"),
        },
        {
          src: require("../assets/carnaval03.jpg"),
        },
        {
          src: require("../assets/carnaval04.jpg"),
        },
      ],
    };
  },
};
</script>