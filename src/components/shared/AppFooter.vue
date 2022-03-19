<template>
    <v-footer
    dark
    padless
  >
    <v-card
      flat
      tile
      class="footer-container grey darken-4 --text text-center"
    >
      <v-card-text>
        <v-btn
          v-for="icon in icons"
          :key="icon"
          class="mx-4 white--text"
          icon
        >
          <v-icon size="24px">
            {{ icon }}
          </v-icon>
        </v-btn>
      </v-card-text>

      <v-card-text class="nwhite--text pt-0 d-flex">
        <label class="d-flex align-center">Assine nossa newsletter:</label> 
        <template>
            <v-text-field class="mx-5" :rules="rules"></v-text-field>
        </template>
        <v-btn color="secondary">
            Assinar
        </v-btn>
      </v-card-text>

      <v-divider></v-divider>

      <v-card-text class="white--text">
        {{ new Date().getFullYear() }} — <strong>copyright ©</strong>
      </v-card-text>
    </v-card>
  </v-footer>    
</template>

<script>
  export default {
    name: 'AppFooter',
    data: () => ({
      icons: [
        'mdi-facebook',
        'mdi-twitter',
        'mdi-linkedin',
        'mdi-instagram',
      ],
      rules: [
        value => !!value || 'Required.',
        value => (value || '').length <= 20 || 'Max 20 characters',
        value => {
          const pattern = /^(([^<>()[\]\\.,;:\s@"]+(\.[^<>()[\]\\.,;:\s@"]+)*)|(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/
          return pattern.test(value) || 'Invalid e-mail.'
        },
      ],
    }),
  }
</script>


<style scoped>
.footer-container{
    min-width: 100%;
}
</style>