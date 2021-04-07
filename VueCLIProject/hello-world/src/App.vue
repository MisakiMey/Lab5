<template>
  <div id="app">
  <img src ="./assets/logo000000.png"/>
  <userdata/>
  <comment/>
  <nameCheck/>
  </div>
</template>

<script>
import userdata from "./components/userdata";
import comment from "./components/comment";
import nameCheck from "./components/Participants";
export default {
  name: 'App',
  components: {
    userdata,
    comment,
    nameCheck,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
#app img {
  height: 500px;
  weight: 500px;
}
</style>
