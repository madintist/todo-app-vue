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
h1 {
    box-sizing: border-box;
    color: inherit;
    display: block;
    font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
    font-weight: 500;
    line-height: 1.1;
    margin-bottom: 10px;
    margin-top: 20px;
    text-size-adjust: 100%;
}
</style>
