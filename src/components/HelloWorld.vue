<template>
  <div id="App">
    <div id="intro">
      <img
        src="https://www.neoenergia.com/pt-br/PublishingImages/cabecalhos/concurso-parodia.png"
      />
      <h1></h1>
      <div class="button">
        <v-btn
          @click="delay"
          color="#F58220"
          elevation="2"
          medium
          outlined
          rounded
        >
          BLOCOS PELO BRASIL
        </v-btn>
      </div>
    </div>
  </div>
</template>

<script>
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
  padding: 10px;
  background-color: #f8f8f8;
  color: rgba(2, 1, 0, 0.781);
  font-family: "Lucida Sans", "Lucida Sans Regular", "Lucida Grande",
    "Lucida Sans Unicode", Geneva, Verdana, sans-serif;
}
.button {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
</style>