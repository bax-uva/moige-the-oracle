<template>
<div class="question">
  <h1>What should I wear?</h1>
</div>
</template>

<script>
export default {
  name: "Header"
};
</script>

<style>
.question {
  display: flex;
  justify-self: center;
  align-self: center;
  width: 80%;
  transform: rotate(-4deg);
  color: black;
  font-size: 1.7em;
  text-align: center;
  text-transform: lowercase;
}

@media screen and (min-width: 450px) {
  .question {
    font-size: 2.2em;
  }
}
</style>
