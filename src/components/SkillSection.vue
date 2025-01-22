<template>
    <section class="skill-section">
      <div class="skills-container">
        <div v-for="skill in skills" :key="skill.id" class="skill-card">
          <img :src="skill.imgSrc" :alt="skill.title" class="skill-icon" />
          <h3 class="skill-title">{{ skill.title }}</h3>
          <p class="skill-description">{{ skill.description }}</p>
        </div>
      </div>
    </section>
  </template>
  
  <script>
  import { skills } from "@/assets/data/skills";
  
  export default {
    name: "SkillSection",
    data() {
      return {
        skills,
      };
    },
  };
  </script>
  
  <style scoped>
  .skill-section {
    font-family: 'Epilogue', sans-serif;
    padding: 5rem 2rem;
    background-color: #f9f9f9;
  }
  
  .skills-container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
    justify-items: center;
  }
  
  .skill-card {
    background-color: transparent;
    text-align: center;
    padding: 1rem;
    width: 100%;
    max-width: 300px;
  }
  
  .skill-icon {
    width: 80px;
    height: 80px;
    margin-bottom: 1rem;
  }
  
  .skill-title {
    font-size: 1.5rem;
    font-weight: 600;
    margin-bottom: 0.5rem;
    color: #333;
  }
  
  .skill-description {
    font-size: 1rem;
    color: #666;
    line-height: 1.5;
  }
  
  .skill-card p,
  .skill-card h3 {
    font-family: 'Epilogue', sans-serif;
  }
  </style>
  