<template>
  <div class="todo-container">
    <page-header :header-text="headerText"></page-header>
    <!-- todo-list -->
    <todo-list></todo-list>
  </div>
</template>

<script>
  import PageHeader from './PageHeader';
  import TodoList from './TodoList';

  export default {
    name: 'todo-container',
    components: {
      'page-header': PageHeader,
      'todo-list': TodoList
    },
    data () {
      return {
        headerText: 'Todo List'
      };
    }
  };
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
* {
    box-sizing: border-box;
}

h1 {
    color: inherit;
    display: block;
    font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
    font-weight: 500;
    line-height: 1.1;
    margin-bottom: 10px;
    margin-top: 20px;
    text-size-adjust: 100%;
}

ul {
    margin-top: 0;
}
</style>
