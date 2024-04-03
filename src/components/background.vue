<template>
    <div class="background">
      <video autoplay muted loop playsinline src="./icons/background.mp4"></video>
    </div>  
  </template>
  
  <style scoped>
  .background {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: -2;
  }
  
  .video-container {
    overflow: hidden;
    object-fit: cover;
    -webkit-background-size: cover; 
    -moz-background-size: cover; 
    -o-background-size: cover; 
    background-size: cover;
    filter: brightness(0.8);
  }
  </style>
  