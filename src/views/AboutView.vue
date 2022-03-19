<template>
  <div class="about">
    <div class="paragrafo" >
      <p class="text-center" >Devido à pandemia não conseguimos nos encontrar para festejarmos juntos, mas mesmo assim não perdemos nossas raízes</p>
    </div>
    
  <v-container class="grey lighten-5">
    <v-row no-gutters>
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
        >
        <div class="nomepart">
          <span>Ariana Almeida</span>
        </div>

           <v-avatar
            class="profile"
            color="grey"
            size="80"
            tile
          >
            <v-img src="@/assets/Ariana.png"></v-img>
            
          </v-avatar>
          
          <p>Algo Sobre</p>
        </v-card>
      </v-col>
      <v-col order="12">
        <v-card
          class="pa-2"
          outlined
          tile
        >
        <div class="nomepart">
          <span>Flavia Passos</span>
        </div>
        
           <v-avatar
            class="profile"
            color="grey"
            size="80"
            tile
          >
            <v-img src="@/assets/Flavia.png"></v-img>
            
          </v-avatar>
          <p>Algo Sobre</p>
        </v-card>
      </v-col>
      <v-col order="12">
        <v-card
          class="pa-2"
          outlined
          tile
        >
        <div class="nomepart">
          <span>Jorcelino Santos</span>
        </div>

        
           <v-avatar
            class="profile"
            color="grey"
            size="80"
            tile
          >
            <v-img src="@/assets/Jorcelino.png"></v-img>
            
          </v-avatar>
          <p>Algo Sobre</p>
        </v-card>
      </v-col>
    </v-row>

    <v-row no-gutters>
      <v-col>
        <v-card
          class="pa-2"
          outlined
          tile
        >
        <div class="nomepart">
          <span>Marco Branco</span>
        </div>
        <v-avatar
            class="profile"
            color="grey"
            size="80"
            tile
          >
            <v-img src="@/assets/Marco.png"></v-img>
            
          </v-avatar>
          <p>Algo Sobre</p>
        </v-card>
      </v-col>
      <v-col order="12">
        <v-card
          class="pa-2"
          outlined
          tile
        >
        <div class="nomepart">
          <span>Pedro Stanislau</span>
        </div>
        <v-avatar
            class="profile"
            color="grey"
            size="80"
            tile
          >
            <v-img src="@/assets/Pedro.png"></v-img>
            
          </v-avatar>
          <p>Algo Sobre</p>
        </v-card>
      </v-col>
      <v-col order="12">
        <v-card
          class="pa-2"
          outlined
          tile
        >
        <div class="nomepart">
          <span>Thays Souza</span>
        </div>
        <v-avatar
            class="profile"
            color="grey"
            size="80"
            tile
          >
            <v-img src="@/assets/Thays.png"></v-img>
            
          </v-avatar>
          <p>Algo Sobre</p>
        </v-card>
      </v-col>
    </v-row>

  </v-container>

  </div>
</template>

<script>
export default {
  
}
</script>

<style scoped>
.paragrafo p{
  margin: 30px;
}

.nomepart span{
    display: flex;
    color:#F58220;
    font-weight: bold;

}

</style>