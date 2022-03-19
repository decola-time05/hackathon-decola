<template>
  <div class="about">
    <div class="paragrafo" >
      <p class="text-center" >O projeto "Carnaval Virtual" foi desenvolvido durante a Edição Luna do Hackaton Decola Iteris promovido pela <a href="https://www.iteris.com.br">Iteris</a></p>
      <h2 class="text-center">Conheça os desenvolvedores</h2>
    </div>
    
  <v-container class="grey lighten-5">
    <v-row no-gutters>
      <v-col>
        <v-card
          class="pa-2 tamCard"
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
          
          <p>Xangri-Lá - RS</p>
        </v-card>
      </v-col>
      <v-col order="12">
        <v-card
          class="pa-2 tamCard"
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
          <p>Recife - PE</p>
        </v-card>
      </v-col>
      <v-col order="12">
        <v-card
          class="pa-2 tamCard"
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
          <p>Uberaba - Mg</p>
        </v-card>
      </v-col>
    </v-row>

    <v-row no-gutters>
      <v-col>
        <v-card
          class="pa-2 tamCard"
          outlined
          tile
        >
        <div class="nomepart">
          <span>Marco Branco</span>
        </div>
        <v-avatar
            class="profile"
            color="grey"
            size="75"
            tile
          >
            <v-img src="@/assets/Marco.png"></v-img>
            
          </v-avatar>
          <p>Ribeirão Preto -SP </p>
          
        </v-card>
      </v-col>
      <v-col order="12">
        <v-card
          class="pa-2 tamCard"
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
          <p class="nomecidade">Novo Hamburgo - RS</p>
        </v-card>
      </v-col>
      <v-col order="12">
        <v-card
          class="pa-2 tamCard"
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
          <p class="nomecidad">Fortaleza - CE</p>
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
    font-size: 12px;

}

.nomecidade{

  font-size: 14px;
}

.tamCard{

  max-height: 163px;
}


</style>