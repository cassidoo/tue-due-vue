<template>
  <div class="counter">
    Counter: <br />

    We are going to count: {{ count }}
    <br />

    <button @click="add">Click me to up the count!</button>
    
    <br />
    <button @click="subtract">Click me to sink the count!</button>
  </div>
</template>

<script>
export default {
  name: 'Counter',
  props: {
  },
  data() {
    return {
      count: 0
    }
  },
  methods: {
    add() {
      this.count++
    },
    subtract() {
      this.count--
    },
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .counter {
    background: #A3BE8C;
    padding: 20px;
  }
  .counter button {
    background: #ECEFF4;
    border-radius: 10px;
    border: 0;
  }
</style>
