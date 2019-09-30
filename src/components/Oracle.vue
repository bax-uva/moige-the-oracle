<template>
<div class="main">
  <div class="margin left-margin">
    <div class="inner-left"></div>
  </div>
  <div class="oracle-area">
    <div class="inner-oracle-area">
      <Question />
      <Answer />
    </div>
  </div>
  <div class="margin right-margin">
    <div class="inner-right"></div>
  </div>
</div>
</template>

<script>
import Question from "./Question.vue";
import Answer from "./Answer.vue";

export default {
  name: "Oracle",
  props: {
    msg: String
  },
  components: {
    Question,
    Answer
  }
};
</script>

<style>
.main {
  width: 100%;
  display: flex;
  padding-top: 2em;
  height: 50vh;
}

.margin {
  width: 2em;
  height: 50vh;
}

.left-margin {
  background-color: #ff8f64e3;
}

.inner-left {
  width: 100%;
  height: 50vh;
  background: rgba(80, 200, 255, 0.6);
  transform: rotate(-6deg);
  position: relative;
  top: 0px;
  left: 10px;
}

.right-margin {
  background-color: #590059;
}

.inner-right {
  width: 100%;
  height: 50vh;
  background: rgba(255, 255, 0, 0.5);
  transform: rotate(3deg);
  position: relative;
  top: 8px;
}

.oracle-area {
  background-color: #40d086;
  width: 100%;

}

.inner-oracle-area {
  width: 100%;
  height: 50vh;
  background: rgba(255, 0, 255, 0.5);
  transform: rotate(3deg);
  position: relative;
  top: 5px;
  left: 0px;
  display: flex;
  flex-direction: column;
}

@media screen and (min-width: 450px) {
  .margin {
    width: 30%;
  }
}

@media screen and (min-width: 800px) {}
</style>
