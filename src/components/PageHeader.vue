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
    color: inherit;
    font-family: inherit;
    font-size: 36px;
    font-weight: 500;
    line-height: 1.1;
    margin: 0.67em 0;
    margin-bottom: 10px;
    margin-top: 20px;
    text-align: center;
    width: 100%;
}
</style>
