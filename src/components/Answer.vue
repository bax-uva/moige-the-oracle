<template>
<div class="answer">
  <p class="entry entry1"></p>
  <p class="entry entry2"></p>
  <p class="entry entry3"></p>
  <p class="entry entry4"></p>
  <p class="entry entry5"></p>
  <p class="entry entry6"></p>
</div>
</template>

<script>
export default {
  name: "Answer"
};
</script>

<style>
.answer {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  min-height: auto;
  display: block;
}

.entry {
  color: white;
  height: 50px;
  font-size: 1em;
  font-family: "Lato", sans-serif;
}

.answer {
  padding-left: 1em;
  padding-top: 1em;
  padding-right: 0.5em;
}

.entry {
  padding-bottom: 0.5em;
}
</style>
