<template>
    <section class="gallery-section">
      <div class="container">
        <h2 class="section-title">Latest work</h2>
        <div class="gallery-grid">
          <div v-for="item in gallery" :key="item.id" class="gallery-item">
            <img :src="item.imgSrc" :alt="item.title" class="gallery-image" />
            <div class="text">
              <h3 class="title">{{ item.title }}</h3>
              <p class="category">{{ item.category }}</p>
            </div>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script>
  import { gallery } from "@/assets/data/gallery";
  
  export default {
    name: "GallerySection",
    data() {
      return {
        gallery,
      };
    },
  };
  </script>
  
  <style scoped>
  .gallery-section {
    font-family: 'Epilogue', sans-serif;
    padding: 4rem 0;
    background-color: #f8f9fa;
  }
  
  .container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 1rem;
  }
  
  .section-title {
    font-size: 2rem;
    font-weight: 700;
    text-align: center;
    margin-bottom: 2rem;
    color: #333;
  }
  
  .gallery-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr); 
    gap: 2rem; 
  }
  
  .gallery-item {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
  }
  
  .gallery-image {
    width: 100%;
    height: auto;
    border: none;
    margin-bottom: 1rem;
  }
  
  .text {
    text-align: left;
  }
  
  .title {
    font-size: 1.2rem;
    font-weight: 700;
    margin-bottom: 0.5rem;
    color: #000;
  }
  
  .category {
    font-size: 0.9rem;
    color: #555;
  }
  .gallery-card p {
  font-family: 'Epilogue', sans-serif;
}
  </style>
  