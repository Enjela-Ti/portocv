<template>
  <div class="background">
    <background />
  </div>

  <div class="profile">
    <profile />
  </div>

  <h1>Enjela Maharani</h1>

  <div class="buton-About">
    <butAbo />
  </div>

  <div class="button">
    <tombol />
  </div>

  <div class="paragraf">
    <paragraf />
  </div>

  <div class="svg1">
    <svg1 />
  </div>
</template>

<script>
import background from './components/background.vue';
import Profile from './components/Profile.vue'; 
import butAbo from './components/butAbo.vue';
import button1 from './components/button1.vue'; 
import paragraf from './components/Paragraf.vue';
import svg1 from './components/icons/svg.vue';

export default {
  name: 'App',
  components: {
    background,
    Profile, 
    butAbo,
    tombol: button1,
    paragraf,
    svg1
  }
}
</script>

<style>
h1{
  position: fixed;
  left: 21%;
  top: 50%;
}

.svg1 {
  display: flex;
  align-items: center; 
  justify-content: center; 
  position: fixed;
  bottom: 0;
  right: 0;
  top: -400px;
  padding: 0 10px;
  z-index: 3;
 }

 .svg1 > * { 
  margin-left: -100px; 
  width: 5px; 
  height: auto; 
  filter: drop-shadow(0 0 10px #fff);
 }
</style>
