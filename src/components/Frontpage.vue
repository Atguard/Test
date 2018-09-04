<template>
  <div class="Root">
    <h1>Game Translation</h1>
    <hr />
    <div class="login-container">
    <h2>Login</h2>
    <br />
    <div id="Username">
    Username:
    <input v-model="user">
    </div>
    <div id="Password">
    Password:
    <input v-model="pw">
    </div>
    </div>
  </div>
</template>

<script>

export default {
 
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  font-family: Courier New, Courier, monospace;
  font-size: 40px;
  background: -webkit-linear-gradient(#FFE400, #E58600);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

hr {
    height: 12px;
    border: 0;
    box-shadow: inset 0 12px 6px -12px rgba(229, 134, 0, 0.5);
}

.login-container {
  //background-color: black;
  margin: auto;
  margin-top: 10%;
  height: 300px;
  width: 350px;
}

.login-container h2 {
  font-family: Courier New, Courier, monospace;
  text-transform: uppercase;
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
