<template>
  <div class="Header">
    <h1>Game Translation</h1>
    <hr>
    <br />
  </div>
</template>

<script>

export default {
  components: {
  },
  name: "Banner",
  data() {
    return {
      date: (new Date()).toLocaleString(),
      user: ""
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  font-size: 52px;
  background: -webkit-linear-gradient(#FFE400, #E58600);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

hr {
    border: 0;
    border-top: solid 1px #ddd;
}

ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 5px;
}
a {
  color: #42b983;
}
</style>
