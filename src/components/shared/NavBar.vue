<template>
  <div class="app-top-bar">

    <v-app-bar app color="#F58220" dark>
      <v-app-bar-nav-icon @click="drawer = true"></v-app-bar-nav-icon>
      <v-toolbar-title>
          Carnaval Virtual
      </v-toolbar-title>
      <v-img   max-height="30" max-width="40" src="../../assets/logo.png" />
    </v-app-bar>

    <v-navigation-drawer v-model="drawer" absolute temporary>
      <v-list nav dense>
        <v-list-item-group v-model="group" active-class="indigo--text text--lighten-2">
    
          <router-link to="/">
            <v-list-item>
              <v-list-item-icon>
                <v-icon>mdi-home</v-icon>
              </v-list-item-icon>
              <v-list-item-title>
                Início
              </v-list-item-title>
            </v-list-item>
          </router-link>

          <router-link to="/carnaval">
            <v-list-item>
              <v-list-item-icon>
                <v-icon>mdi-account</v-icon>
              </v-list-item-icon>
              <v-list-item-title>
                Blocos de carnaval
              </v-list-item-title>
            </v-list-item>
          </router-link>

        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
  </div>
</template>

<script>
export default {
  name: 'AppTopBar',
  data() {
    return {
      drawer: false,
      group: null,
    }
  }
}
</script>

<style scoped>

.logodiv img{ 

  height:30px;
  width:40px;
}

.app-top-bar a {
  text-decoration: none;
}
</style>
