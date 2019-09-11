// App.vue

<template>
  <div id="app">
    <page-template>
      <template #header="">
        <h3>Page Header</h3>
      </template>

      <template #content="">
        <h3>Page Content</h3>
      </template>

      <template #footer="">
        <h3>Page Footer</h3>
      </template>
    </page-template>
  </div>
</template>


<script>
import PageTemplate from "./components/PageTemplate.vue";
export default {
  name: "app",
  components: {
    PageTemplate
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
