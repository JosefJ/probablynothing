<template>
  <div id="app" >
    <img id="horse" src="./assets/horse.png">
    <Content />
  </div>

</template>

<script>
import Content from "@/components/Content";

export default {
  name: 'App',
  components: {
    Content
  },
  data () {
    return {
    }
  },
  methods: {
  }
}
</script>

<style>
@import "./styles/normalize.css";
@import "./styles/skeleton.css";

html, body {
  height: 100%;
  width: 100%;
  padding: 0;
  margin: 0;
  overflow: clip;
}

#horse {
  position: absolute;
  bottom: 0;
  left: 0;
  height: 66vh;
}

#app {
  font-family: "Roboto", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #ffffff;
  background-image: url("./assets/BG.jpg");
}

.columns, .column {
  text-align: justify;
}

h1, h2, h3, h4 {
  text-align: center;
}

p {
  text-align: justify;
  font-size: 18px;
}

</style>
