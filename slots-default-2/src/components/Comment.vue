// Comment.vue

<template>
  <div>
    <div>black text from Comment.vue, from outside the slot</div>
    <slot></slot>
  </div>
</template>

<script>
export default {
  name: 'Comment',
}
</script>

