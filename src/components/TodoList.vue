<template>
  <ul class="list-group">
    <li class="list-group-item">1</li>
    <li class="list-group-item">2</li>
    <li class="list-group-item">3</li>
    <li class="list-group-item">4</li>
  </ul>
</template>

<script>
  export default {
    name: 'todo-list'
  };
</script>

<style scoped>
li {
    display: block;
    position: relative;
}
ul {
    margin-bottom: 20px;
    padding-left: 0;
}
</style>
