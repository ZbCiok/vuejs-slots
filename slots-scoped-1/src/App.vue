<template>
  <div id="app">
    <my-car v-slot="{car}">
      My car:&nbsp;{{ car.name }}
    </my-car>
  </div>
</template>

<script>
import MyCar from "./components/MyCar";

export default {
  name: "app",
  components: {
    MyCar
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
  margin-top: 60px;
}
</style>

