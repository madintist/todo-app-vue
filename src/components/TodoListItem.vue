<template>
  <li>
    {{ todoItem.title }}
  </li>
</template>

<script>
  export default {
    name: 'todo-list-item',
    props: [
      'todo-item'
    ]
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
</style>
