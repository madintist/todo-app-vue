<template>
  <ul>
    <todo-list-item v-for="item in todoItems" :todo-item="item" :key="item.id"></todo-list-item>
  </ul>
</template>

<script>
  import TodoListItem from './TodoListItem';

  export default {
    name: 'todo-list',
    components: {
      'todo-list-item': TodoListItem
    },
    data () {
      return {
        todoItems: [
          {
            id: 0,
            title: 'Item 1'
          },
          {
            id: 1,
            title: 'Item 2'
          },
          {
            id: 2,
            title: 'Item 3'
          },
          {
            id: 3,
            title: 'Item 4'
          }
        ]
      };
    }
  };
</script>

<style scoped>
ul {
    margin-bottom: 20px;
    margin-left: auto;
    margin-right: auto;
    max-width: 400px;
    padding-left: 0;
}
</style>
