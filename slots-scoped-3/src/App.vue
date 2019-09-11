// App.vue

<template>
  <div id="app">
    <CarList :items="['Toyota', 'Fiat', 'Ford', 'Syrenka']">      
      <template slot-scope="{ items }">
        <p v-for="item in items" :key="item">{{ item }}</p>
      </template>
    </CarList>
  </div>
</template>

<script>
import CarList from "./components/CarList.vue";

export default {
  name: "app",
  components: { 
    CarList 
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
