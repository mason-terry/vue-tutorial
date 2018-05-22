<template>
  <div class="home">
    <h1>To Do List</h1>
    <h2>Add a to do</h2>
    <input type='text' />
    <button v-on:click='addItem'>Add</button>
    <ol>
      <li v-for='item in list' v-bind:key='item' v-text='item'></li>
    </ol>
  </div>
</template>

<script>
export default {
  name: 'Home',
  data() {
    let list = ['hello']
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
