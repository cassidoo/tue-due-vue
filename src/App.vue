<template>
  <HelloWorld msg="Do you like the Vue 😏"/>
  <TueDue />
  <Counter />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import TueDue from './components/TueDue.vue'
import Counter from './components/Counter.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    TueDue,
    Counter
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
