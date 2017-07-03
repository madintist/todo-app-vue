<template>
  <ul>
    <li>1</li>
    <li>2</li>
    <li>3</li>
    <li>4</li>
  </ul>
</template>

<script>
  export default {
    name: 'todo-list'
  };
</script>

<style scoped>
li {
    background-color: #fff;
    border: 1px solid #ddd;
    display: block;
    margin-bottom: -1px;
    padding: 10px 15px;
    position: relative;
}
li:first-child {
    border-top-left-radius: 4px;
    border-top-right-radius: 4px;
}

ul {
    margin-bottom: 20px;
    margin-left: auto;
    margin-right: auto;
    max-width: 400px;
    padding-left: 0;
}
</style>
