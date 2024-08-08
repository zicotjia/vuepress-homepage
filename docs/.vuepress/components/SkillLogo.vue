<template>
    <div class="logo-with-text">
      <img :src="image" class="logo" />
      <span class="text">{{ text }}</span>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      image: {
        type: String,
        required: true
      },
      text: {
        type: String,
        required: true
      }
    }
  };
  </script>
  
  <style scoped>
  .logo-with-text {
    display: inline-flex;
    align-items: center;
  }
  
  .logo {
    max-width: 25px;
    height: 15px;
    margin-right: 5px;
  }
  
  .text {
    font-size: 15px;
    align-self: self-end;
  }
  </style>