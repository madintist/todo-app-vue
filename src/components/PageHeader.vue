<template>
  <h1>{{ headerText }}</h1>
</template>

<script>
  export default {
    name: 'page-header',
    props: [
      'header-text'
    ]
  };
</script>

<style scoped>
h1 {
    font-size: 36px;
    margin: 0.67em 0;
    text-align: center;
}
</style>
