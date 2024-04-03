<template>
    <div class="profile">
      <img src="./icons/profile.png" alt="Profile Picture">
    </div>
  </template>
  
  <style scoped>
  .profile {
    position: fixed;
    top: 10%;
    left: 20%; 
    transform: translate(-20%, -20%);
    animation: zoom 2s ease infinite alternate;
  }
  
  .profile img {
    width: 250px;
    height: auto;
  }
  
  @keyframes zoom {
    from {
      transform: scale(1);
    }
    to {
      transform: scale(1.2);
    }
  }
  </style>
  