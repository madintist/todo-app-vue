<template>
  <ul>
    <todo-list-item v-for="item in incompleteItems" :todo-item="item" :key="item.id"></todo-list-item>
  </ul>
</template>

<script>
  import TodoListItem from './TodoListItem';

  export default {
    name: 'todo-list',
    components: {
      'todo-list-item': TodoListItem
    },
    computed: {
      incompleteItems () {
        return this.todoItems.filter(function (item) {
          return !item.complete;
        });
      }
    },
    data () {
      return {
        todoItems: [
          {
            id: 0,
            title: 'Item 1',
            complete: false
          },
          {
            id: 1,
            title: 'Item 2',
            complete: false
          },
          {
            id: 2,
            title: 'Item 3',
            complete: false
          },
          {
            id: 3,
            title: 'Item 4',
            complete: false
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
