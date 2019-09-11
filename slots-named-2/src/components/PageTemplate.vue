// PageTemplate.vue

<template>
  <div>
    <header>
      <slot name="header" />
    </header>

    <main>
      <slot name="content"/>
    </main>

    <footer>
      <slot name="footer" />
    </footer>
  </div>
</template>

<script>
export default {};
</script>
