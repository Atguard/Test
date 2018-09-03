<template>
  <div class="Login">
  <!--
    <h1>Game Translating</h1>
    Hallo{{ user && ' '+user }}! Am {{date}} begrüße ich dich!
    <br />
    <input v-model="user" />
    <button @click="refresh2">Refresch</button>
  -->
  </div>
</template>

<script>
export default {
  components: {},
  name: "Banner",
  data() {
    return {
      date: new Date().toLocaleString(),
      user: ""
    };
  },
  methods: {
    refresh2: function() {
      this.user = "";
      this.refresh();
    },
    refresh: function() {
      this.date = new Date().toLocaleString();
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  font-size: 48px;
  background: -webkit-linear-gradient(#ffe400, #e58600);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

.shadow {
  -moz-box-shadow: 3px 3px 5px 6px #ccc;
  -webkit-box-shadow: 3px 3px 5px 6px #ccc;
  box-shadow: 3px 3px 5px 6px #ccc;
}

h2 {
  font-weight: bold;
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
