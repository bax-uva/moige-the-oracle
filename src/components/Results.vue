<template>
  <p class="entry">
    {{ item[[Math.floor(Math.random() * item.length)]] }}
  </p>
</template>

<script>
export default {
  name: "Results",
  props: ["item"]
};
</script>

<style>
.answer {
  margin-top: 3em;
}

.answer p {
  /* background: rgba(170, 170, 170, 0.7); */
  display: flex;
  justify-content: space-between;
  border-bottom: 0.5px solid white;
  padding: 0.3em;
  z-index: 10;
  color: black;
  font-size: 1em;
  font-family: "Lato", sans-serif;
  text-transform: uppercase;
}
</style>
