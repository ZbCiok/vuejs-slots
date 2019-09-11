// MyCar.vue

<template>
  <span>
    <slot v-bind:car="car">
      {{ car.name }}
    </slot>
  </span>
</template>

<script>
export default {
  data () {
    return {
      car: { "name": "Syrenka" }
    }
  }
}
</script>