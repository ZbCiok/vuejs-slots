// app.vue

<template>
  <div id="app">
    <Comment>
      <span class="text-red">red text from the slot<br>
      (default slot)</span>
    </Comment>
  </div>
</template>

<script>
import Comment from './components/Comment'

export default {
  name: 'app',
  components: {
    Comment
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.text-red {
  color: red;
}
</style>

