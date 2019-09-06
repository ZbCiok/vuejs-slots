<template>
  <div id="app">
    <my-named-slot>
      <h1 slot="title">Title: Named Slot</h1>
      <p slot="description">
        Description: 'slot' element has a special attribute, 
        'name', which can be used to define additional slots.
      </p>
    </my-named-slot>
  </div>
</template>

<script>
import MyNamedSlot from "./components/MyNamedSlot.vue";
export default {
  name: "app",
  components: {
    MyNamedSlot
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

