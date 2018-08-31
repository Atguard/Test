<template>
  <div class="Test">
    <h1>{{ msg }}</h1>
    Hallo{{ user && ' '+user }}! Am {{date}} begrüße ich dich!
    <br />
    <input v-model="user" />
    <button @click="refresh2">Refresch</button>
  </div>
</template>

<script>

export default {
  components: {
  },
  name: "Banner",
  data() {
    return {
      msg: "Welcome to ... what ever!",
      date: (new Date()).toLocaleString(),
      user: ""
    };
  },
  methods: {
    refresh2: function() {
      this.user = ""
      this.refresh()
    },
    refresh: function() {
      this.date = (new Date()).toLocaleString()
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

<!--
Some colors:
00B28B
04FFC7
00FFC6
B22D00
FF4100
-->
<style scoped>
h1 {
  color: #B22D00;
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
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
