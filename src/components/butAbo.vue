<template>
    <div class="button">
      <button @click="toggleAbout" class="show-hide-btn">{{ buttonLabel }}</button>
      <transition name="slide">
        <p v-if="showAbout" class="about" style="color: white; font-weight: bold;">Saya adalah seorang programer dan saya memiliki pengalaman <br>dalam pengembangan perangkat lunak. 
      Saya ahli dalam bahasa<br> pemrograman seperti JavaScript, Python, dan Java. 
      Selain itu,  <br>saya juga memiliki keahlian dalam pengembangan web menggunakan  <br>framework seperti Vue.js dan React.
      Saya tertarik untuk terus belajar  <br>dan meningkatkan keterampilan saya dalam industri teknologi.</p>
      </transition>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        showAbout: false
      };
    },
    computed: {
      buttonLabel() {
        return this.showAbout ? 'Hide About' : 'Show About';
      }
    },
    methods: {
      toggleAbout() {
        this.showAbout = !this.showAbout;
      }
    }
  };
  </script>
  
  <style scoped>
  .show-hide-btn {
    padding: 10px 20px;
    background-color: transparent;
    backdrop-filter: blur(10px);
    color: #fff;
    border: 2px solid gray;
    cursor: pointer;
  }
  
  .about {
    margin-top: 0px;
    padding: 10px;
  }
  
  .slide-enter-active,
  .slide-leave-active {
    transition: transform 0.5s ease;
  }
  
  .slide-enter {
    transform: translateX(-100%);
  }
  
  .slide-leave-to {
    transform: translateX(100%);
  }

  .button{
    position: fixed;
    top: 60%;
    left: 22%; 
  }
  </style>
  