// CarList.vue

<template>
  <div>
    <p><input v-model="inputFilter" /></p>
    <slot v-bind:items="filteredList" />
  </div>
</template>

<script>
export default {
  props: ["items"],
  data: () => ({
    inputFilter: ""
  }),
  computed: {
    filteredList() {
      return this.items.filter(item => item.includes(this.inputFilter));
    }
  }
};
</script>
