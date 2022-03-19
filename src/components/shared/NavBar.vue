<template>
  <div class="app-top-bar">
    <v-app-bar app color="#F58220" dark>
      <v-app-bar-nav-icon @click="drawer = true"></v-app-bar-nav-icon>
      <v-toolbar-title> Carnaval Virtual </v-toolbar-title>
      <v-avatar size="55" class="ml-auto" tile>
        <img src="../../assets/logo.png" alt="" />
      </v-avatar>
    </v-app-bar>

    <v-navigation-drawer v-model="drawer" fixed temporary color="rgb(245, 140, 32, 0.95)">
      <v-list nav dense>
        <v-list-item-group
          v-model="group"
          active-class="white--text"
        >
          <router-link to="/">
            <v-list-item>
              <v-list-item-icon>
                <v-icon>mdi-home</v-icon>
              </v-list-item-icon>
              <v-list-item-title> Início </v-list-item-title>
            </v-list-item>
          </router-link>

          <router-link to="/carnaval">
            <v-list-item>
              <v-list-item-icon>
                <v-icon>mdi-account</v-icon>
              </v-list-item-icon>
              <v-list-item-title> Blocos de carnaval </v-list-item-title>
            </v-list-item>
          </router-link>
        <v-container class="mt-16">
          <router-link to="/about">
            <v-list-item>
              <v-list-item-icon>
                <v-icon>mdi-information</v-icon>
              </v-list-item-icon>
              <v-list-item-title> Sobre nós </v-list-item-title>
            </v-list-item>
          </router-link>
        </v-container>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
  </div>
</template>

<script>
export default {
  name: "AppTopBar",
  data() {
    return {
      drawer: false,
      group: null,
    };
  },
};
</script>

<style scoped>
.logodiv img {
  height: 30px;
  width: 40px;
}

.app-top-bar a {
  text-decoration: none;
}
</style>
