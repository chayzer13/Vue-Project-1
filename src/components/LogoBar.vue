<template>
    <section class="logo-bar">
      <div class="logo-container">
        <img 
          v-for="logo in logos" 
          :key="logo.id" 
          :src="logo.imgSrc" 
          :alt="logo.alt" 
          class="logo"
        />
      </div>
    </section>
  </template>
  
  <script>
  import { logos } from '@/assets/data/logos'; 
  
  export default {
    name: 'LogoBar',
    data() {
      return {
        logos,
      };
    },
  };
  </script>
  
  <style scoped>
  .logo-bar {
    font-family: 'Epilogue', sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 2rem 0;
    background-color: #f9f9f9; 
  }
  
  .logo-container {
    display: flex;
    gap: 10rem; 
    justify-content: center;
    align-items: center;
  }
  
  .logo {
    width: 90px; 
    height: 50px; 
    object-fit: contain; 
    transition: transform 0.3s ease;
  }
  
  .logo:hover {
    transform: scale(1.1); 
  }
  </style>
  
  