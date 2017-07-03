<template>
  <div class="todo-container">
    <page-header :header-text="headerText"></page-header>
    <!-- todo-list -->
  </div>
</template>

<script>
  import PageHeader from './PageHeader';

  export default {
    name: 'todo-container',
    components: {
      'page-header': PageHeader
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
</style>
