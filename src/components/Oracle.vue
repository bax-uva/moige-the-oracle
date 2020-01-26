<template>
<div>
  <div class="main">
    <div class="margin left-margin">
      <div class="inner-left"></div>
    </div>
    <div class="oracle-area">
      <div class="inner-oracle-area">
        <Header />
        <div class="answer">
          <Results v-for="item in data.outfits" v-bind:item="item" />
        </div>
      </div>
    </div>
    <div class="margin right-margin">
      <div class="inner-right"></div>
    </div>
  </div>
  <Reset />
</div>
</template>

<script>
import Header from "./Header.vue";
import Results from "./Results.vue";
import Reset from "./Reset.vue";
import data from "../data/data.js";
export default {
  name: "Oracle",
  components: {
    Header,
    Results,
    Reset
  },
  data() {
    return {
      data
    };
  },
  props: {
    item: String
  }
};
</script>

<style>
.main {
  width: 100%;
  display: flex;
  padding-top: 2em;
  height: 100vh;
  z-index: 0;
  flex-grow: 1;
}

.margin {
  width: 2em;
  height: 50vh;
  z-index: 0;
}

.left-margin {
  background: rgba(80, 200, 255, 0.9);
  z-index: 0;
}

.inner-left {
  width: 100%;
  height: 50vh;
  background-color: rgba(255, 143, 100, 0.7);
  transform: rotate(-6deg);
  position: relative;
  top: 0px;
  left: 10px;
  z-index: 0;
}

.right-margin {
  background-color: rgba(70, 0, 51, 0.8);
  z-index: 0;
}

.inner-right {
  width: 100%;
  height: 50vh;
  background: rgba(255, 255, 0, 0.6);
  transform: rotate(2deg);
  position: relative;
  top: 15px;
  left: -2px;
  z-index: 0;
}

.oracle-area {
  background: rgba(208, 64, 138, 0.6);
  width: 100%;
  z-index: 0;
}

.inner-oracle-area {
  padding: 0 2em 0 1em;
  width: 102%;
  height: 100vh;
  background-color: rgba(64, 208, 134, 0.4);
  transform: rotate(4deg);
  position: relative;
  top: -8px;
  left: 8px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  z-index: 4;
}

@media screen and (min-width: 450px) {
  .margin {
    width: 30%;
  }
}
</style>
