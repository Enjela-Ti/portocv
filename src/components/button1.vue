<template>
    <div class="button-container">
      <button class="home-btn">Home</button>
      <button class="exit-btn">Exit</button>
    </div>
  </template>
  
  <script>
  export default {
    name: 'TopButtons'
  }
  </script>
  
  <style scoped>
  .button-container {
    position: fixed;
    top: 10px;
    left: 50%;
    transform: translateX(-50%);
  }
  
  .home-btn,
  .exit-btn {
    padding: 10px 20px;
    margin: 0 10px;
    background-color: transparent;
    color: #fff;
    border: 2px solid grey;
    cursor: pointer;
    transition: background-color 0.3s;
  }
  
  .home-btn:hover,
  .exit-btn:hover {
    background-color: rgba(128, 128, 128, 0.3);
  }
  </style>
  