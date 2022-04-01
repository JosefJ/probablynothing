<template>
  <div id="content" class="container">

    <simple-modal v-model="isShow" title="Modal Header">
<!-- TODO: here comes the Rickroll modal -->
    </simple-modal>

    <div class="hero row">
      <div class="twelve columns stick">
        <img id="Logo" src="../assets/dcivi-logo2.png">
        <div>
          <h1> October 2022, Prague, CZ </h1>
        </div>
        <a href="" target="_blank">
          <br>
          <button id="sign" @click="isShow = !isShow">
            Get Tickets
          </button>
        </a>
      </div>

    </div>
  </div>

</template>

<script>
import SimpleModal from 'simple-modal-vue';

export default {
  name: 'Content',
  components: {
    SimpleModal
  }
  ,methods: {
  }, mounted() {
  },
  data() {
    return {
      isShow: false
    }
  }
}



</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.container {

}

.row {
  text-align: center;
}

#content {

}

#Logo {
  /*filter: brightness(0) invert(1);*/
  margin-bottom: 1vh;
  width: 100%;
}

.stick {
  position: sticky;
  top: 20vh;
  margin-bottom: 50px;
}

.hero {
  height: 100vh;
}

.columns, .column {
  text-align: center;
}
h1 {
  color: #000000;
}
button {
  border: 2px #ffffff solid;
  border-radius: 45px;
  width: 350px;
  font-size: 24px;
  background: #FFFFFF;
  color: #000000;
  height: 60px;
  /*padding: 40px 40px 40px 40px;*/
  /*filter: saturate(0);*/
  /*!*opacity: 0.5*!*/
}

button:hover {
  opacity: 1;
  background: #000000;
  color: #FFFFFF;
  border: #000000;
}

@media (min-width:1920px) {
  #HFC {
    width: 710px;
  }
}

@media (max-width:720px) {
  .hero {

  }
}

</style>
