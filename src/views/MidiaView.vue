<template>
    <v-container>
    <div class="frame">
        <iframe
          class="responsive-iframe"
          width="560"
          height="315"
          src="https://www.youtube.com/embed/PB6qcm2raow"
          title="YouTube video player"
          frameborder="0"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
          allowfullscreen
        ></iframe>
    </div>

    <v-col class="my-6">
    <iframe style="border-radius:12px"
    src="https://open.spotify.com/embed/playlist/7Hu1eSuTkxBAQ3VhszGgDd?utm_source=generator" 
    width="100%" height="380" frameBorder="0" 
    allowfullscreen="" allow="autoplay; 
    clipboard-write; encrypted-media; 
    fullscreen; picture-in-picture">
    </iframe>
      </v-col>
    </v-container>
</template>
<script>
export default {
  name: "MidiaView",
};
</script>
<style scoped>
.frame {
  position: relative;
  overflow: hidden;
  width: 100%;
  padding-top: 56.25%; 
}
.responsive-iframe {
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  width: 100%;
  height: 100%;
}
</style>