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

      <v-card-text class="nwhite--text pt-0">
        <div class="newsletter d-flex align-center mx-auto">
            <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1" width="24" height="24" viewBox="0 0 24 24"><path d="M5,3H19A2,2 0 0,1 21,5V19A2,2 0 0,1 19,21H5A2,2 0 0,1 3,19V5A2,2 0 0,1 5,3M7.5,15A1.5,1.5 0 0,0 6,16.5A1.5,1.5 0 0,0 7.5,18A1.5,1.5 0 0,0 9,16.5A1.5,1.5 0 0,0 7.5,15M6,10V12A6,6 0 0,1 12,18H14A8,8 0 0,0 6,10M6,6V8A10,10 0 0,1 16,18H18A12,12 0 0,0 6,6Z" /></svg>
            <template>
            <label>Assine nossa newsletter:</label> 
                <v-text-field class="mx-3" :rules="rules"></v-text-field>
            </template>
        </div>
        <div class="button-assinar mx-auto">
            <v-btn color="primary my-3 mx-3">
                        Assinar
            </v-btn>
        </div>
        
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
      iconRss: 'mdi-rssbox',
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
.newsletter, .button-assinar{
    max-width: 500px;
}
.button-assinar{
    text-align: right;
}
svg{
    fill: orange;
    margin: 0px 5px;
}
</style>