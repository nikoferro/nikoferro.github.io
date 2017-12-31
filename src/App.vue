<template>
  <div id="app">
    <Header/>
  </div>
</template>

<script>
import "font-awesome/css/font-awesome.css";
import Header from "./components/Header";

export default {
  name: "app",
  components: {
    Header
  }
};
</script>

<style>
html,
body {
  height: 100%;
  padding: 0px;
  margin: 0px;
}
#app {
  height: 100%;
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  display: flex;
  flex-direction: column;
  justify-content: center;
}
</style>
