<template>
  <div class="answer">
    <p class="entry">
      item
    </p>
  </div>
</template>

<script>
export default {
  name: "Answer"
};
</script>

<style>
.answer {
  /* background: rgba(170, 170, 170, 0.7); */
  display: flex;
  justify-content: space-between;
  border-top: 0.5px solid white;
  padding: 0.3em;
  z-index: 10;
  color: black;
  font-size: 1em;
  font-family: "Lato", sans-serif;
  text-transform: uppercase;
  text-align: justify;
}

.entry {
  height: auto;
  max-width: 70%;
}
</style>
