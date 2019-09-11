// app.vue

<template>
  <div id="app">
    <my-default-slot>
      <h1>Default Slot</h1>
    </my-default-slot>
  </div>
</template>

<script>
import MyDefaultSlot from "./components/MyDefaultSlot.vue";
export default {
  name: 'app',
  components: {
    MyDefaultSlot
  }
};
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>