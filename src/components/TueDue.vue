<template>
  <div class="todolist">
    Tue Due in Vue: <br />
    <input type="text" v-model="newItem" @keyup.enter="addItem" />

    <TueDueItem v-for="(item, index) in list" :key="index" :name="item" @delete="removeItem(index)" />
  </div>
</template>

<script>
import TueDueItem from './TueDueItem.vue'

export default {
  name: 'TueDue',
  components: {
    TueDueItem
  },
  data() {
    return {
      list: [
        'sample',
        'thingy'
      ],
      newItem: ''
    }
  },
  methods: {
    addItem() {
      this.list.push(this.newItem)
      this.newItem = ''
    },
    removeItem(index) {
      this.list.splice(index, 1)
    }
  }
}
</script>

<style scoped>
  .todolist {
    background: #B48EAD;
    padding: 20px;
  }
</style>
