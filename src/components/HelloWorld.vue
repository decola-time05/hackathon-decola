<template>
  <div id="intro">
    <img
      src="https://www.neoenergia.com/pt-br/PublishingImages/cabecalhos/concurso-parodia.png"
      alt="A imagem diz Folia em casa, carnaval em segurança. O Folião veste
    adereços carnavalescos dentro de casa."
    />
    <v-container>
      <h3>
        Sabemos que esta data é esperada por muitas pessoas que gostam de curtir
        os blocos de rua, desfiles e festas privadas e, como as celebrações de
        Carnaval para 2022 foram canceladas em boa parte do Brasil,
        desenvolvemos esse aplicativo (ou site) para que possamos sentir o
        gostinho do carnaval e comemorá-lo
        <a href="http://192.168.0.13:8080/midia/">mesmo que em casa!</a>
      </h3>

      <app-carousel />

      <div class="button my-5">
        <v-btn
          @click="delay"
          color="#F58220"
          elevation="2"
          medium
          rounded
          class="white--text"
        >
          BLOCOS PELO BRASIL
        </v-btn>
      </div>
    </v-container>
  </div>
</template>

<script>
import AppCarousel from "../components/AppCarousel.vue";

export default {
  name: "HelloWorld",
  data() {
    return {};
  },
  methods: {
    delay() {
      setTimeout(() => {
        this.$router.push("/carnaval");
      }, 100);
    },
  },
  components: {
    AppCarousel,
  },
};
</script>

<style scoped>
#app {
  background-color: #f6f6f6;
  justify-content: center;
}
img {
  width: 100%;
}
h3 {
  justify-content: center;
  align-items: center;
  background-color: #f8f8f8;
  color: rgba(2, 1, 0, 0.781);
  font-family: "Gill Sans", "Gill Sans MT", Calibri, "Trebuchet MS", sans-serif;
  line-height: 20px;
  text-align: justify;
}
.button {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
</style>