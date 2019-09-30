<template>
  <div id="app">
    <Oracle />
  </div>
</template>

<script>
import Oracle from "./components/Oracle.vue";

export default {
  name: "app",
  components: {
    Oracle
  }
};
</script>

<style>
* {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  font-family: "Archivo", sans-serif;
}

body {
  background-color: #b4b4b4;
  display: flex;
  align-content: center;
  height: 100vh;
}

#app {
  width: 100%;
}

a {
  text-decoration: none;
}
</style>
