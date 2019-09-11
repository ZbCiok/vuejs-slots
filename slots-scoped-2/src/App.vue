// App.vue

<template>
  <div id="app">
    <car-listing>
      <template v-slot:default="slotProps">
        <span>{{ slotProps.car.name }},&nbsp;</span>
        <span>price = {{ slotProps.car.price }}</span>
      </template>
    </car-listing>
  </div>
</template>

<script>
import CarListing from "./components/CarListing";

export default {
  name: "app",
  components: {
    CarListing
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

