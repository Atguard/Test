<template>
  <div id="app">
    <Frontpage/>
  </div>
</template>

<script>
import Frontpage from "./components/Frontpage";

export default {
  name: "App",
  components: {
    Frontpage
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
