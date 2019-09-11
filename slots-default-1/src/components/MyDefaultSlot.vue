// MyDefaultSlot.vue

<template>
  <div>
    <slot>
        <h1>
            No slot is specified in the parent, so this fallback text appears.
        </h1>    
    </slot>
  </div>
</template>

<script>
export default {};
</script>