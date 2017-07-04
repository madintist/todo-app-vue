<template>
  <button @click="completeItem">
    <span></span>
  </button>
</template>

<script>
  export default {
    name: 'complete-item-button',
    props: [
      'target-item'
    ],
    methods: {
      completeItem () 
        this.targetItem.complete = true;
      }
    }
  };
</script>

<style scoped>
button {
    background-color: #5cb85c;
    background-image: none;
    border: 1px solid transparent;
    border-color: #4cae4c;
    border-radius: 4px;
    color: #fff;
    cursor: pointer;
    display: inline-block;
    font-size: 14px;
    font-weight: 400;
    line-height: 1.42857143;
    margin-bottom: 0;
    padding: 6px 12px;
    text-align: center;
    touch-action: manipulation;
    -ms-touch-action: manipulation;
    user-select: none;
    -moz-user-select: none;
    -ms-user-select: none;
    -webkit-user-select: none;
    vertical-align: middle;
    white-space: nowrap;
}

button:active {
    background-color: #449d44;
    background-image: none;
    border-color: #398439;
    box-shadow: inset 0 3px 5px rgba(0, 0, 0, .125);
    color: #fff;
    outline: 0;
}

button:focus {
    color: #fff;
    background-color: #449d44;
    border-color: #255625;
    text-decoration: none;
}

button:hover {
    background-color: #449d44;
    border-color: #398439;
    color: #fff;
    text-decoration: none;
}

span {
    position: relative;
    top: 1px;
    display: inline-block;
    font-family: 'Glyphicons Halflings';
    font-style: normal;
    font-weight: 400;
    line-height: 1;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
}

span::before {
    content: "\e013";
}
</style>
