<template>
  <div class="home">
    <h1>To Do List</h1>
    <h2>Add a todo</h2>
    <input type='text' id='text' />
    <button v-on:click='addItem'>Add</button>
    <ol>
      <li v-for='item in list' v-if='item.done === false' v-bind:key='item'>{{ item.item }} <button v-on:click='item.done = true'>X</button></li>
    </ol>
  </div>
</template>

<script>
let list = [
  //{ item: 'Clean house', done: false },
  //{ item: 'Get groceies', done: false },
  //{ item: 'Walk dog', done: false }
]

export default {
  name: 'Home',
  data() {
    return {
      list: list
    }
  },
  methods: {
    addItem() {
      list.push({ item: document.getElementById('text').value, done: false })
      document.getElementById('text').value = ''
    },
    itemComplete() {
      list.done = true
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
