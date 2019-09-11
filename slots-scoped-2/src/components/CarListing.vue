// CarListing.vue

<template>
  <div class="cars">
    <h1>List of Cars</h1>
    <div>
      <div v-for="car in cars" :key="car.id">
        <slot :car="car"></slot>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      cars: [
        { id: 1, name: "Ford", price: 42000 },
        { id: 2, name: "Toyota", price: 58000 },
        { id: 3, name: "Syrenka", price: 50000 }
      ]
    };
  }
};
</script>