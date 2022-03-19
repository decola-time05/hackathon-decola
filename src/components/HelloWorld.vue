<template>
  <div id="App">
    <div id="intro">
      <img
        src="https://img.freepik.com/fotos-gratis/mascaras-de-mascaras-de-carnaval-e-confetes-com-glitter-dourados-vista-superior-close-up-no-fundo-das-cores-azul-e-laranja_75517-1776.jpg?size=626&ext=jpg"
      />
      <p>
        O carnaval O carnaval O carnaval O carnaval O carnaval O carnaval O
        carnaval O carnaval O carnaval O carnaval O carnaval O carnaval O
        carnaval O carnaval
      </p>
      <div class="botoes">
        <v-btn
          @click="delay"
          color="teal lighten-1"
          elevation="2"
          medium
          outlined
          rounded
        >
          CARDS</v-btn
        >
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
};
</script>

<style scoped>
#app {
  background-color: #f6f6f6;
}
img {
  width: 100%;
}
h1 {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 15px;
  background-color: #070435;
  color: rgba(255, 253, 251, 0.781);
}
</style>