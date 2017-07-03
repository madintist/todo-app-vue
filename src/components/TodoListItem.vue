<template>
  <li>
    {{ todoItem.title }}
    <!-- Complete button here -->
    <complete-item-button></complete-item-button>
  </li>
</template>

<script>
  import CompleteItemButton from './CompleteItemButton';

  export default {
    name: 'todo-list-item',
    components: {
      'complete-item-button': CompleteItemButton
    },
    props: [
      'todo-item'
    ]
  };
</script>

<style scoped>
li {
    align-items: center;
    background-color: #fff;
    border: 1px solid #ddd;
    display: flex;
    justify-content: space-between;
    margin-bottom: -1px;
    padding: 10px 15px;
    position: relative;
}

li:first-child {
    border-top-left-radius: 4px;
    border-top-right-radius: 4px;
}
</style>
