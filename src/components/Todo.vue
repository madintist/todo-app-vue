<template>
  <div class="todo-container">
    <h1>{{ headerText }}</h1>
  </div>
</template>

<script>
export default {
  name: 'hello',
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
  font-weight: normal;
}
</style>
