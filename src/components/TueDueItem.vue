<template>
  <div class="todoitem">
    {{ name }}
    <button @click="$emit('delete')">Done!</button>
  </div>
</template>

<script>
export default {
  name: 'TueDueItem',
  props: {
    name: String
  }
}
</script>

<style scoped>
  .todoitem {
    background: #4C566A;
    color: #ECEFF4;
    padding: 5px;
    margin: 5px;
  }
</style>
