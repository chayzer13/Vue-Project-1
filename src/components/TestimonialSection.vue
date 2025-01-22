<template>
    <section class="testimonial-section">
      <div class="container">
        <h2 class="section-title">Testimonial</h2>
        <div class="testimonials-grid">
          <div v-for="testimonial in testimonials" :key="testimonial.id" class="testimonial-card">
            <p class="testimonial-quote">"{{ testimonial.quote }}"</p>
            <div class="testimonial-card-footer">
              <img :src="testimonial.imgSrc" :alt="testimonial.name" class="testimonial-image" />
              <div class="testimonial-text">
                <div class="testimonial-rating">
                  <span v-for="star in testimonial.rating" :key="star" class="star">★</span>
                  <span v-for="empty in 5 - testimonial.rating" :key="empty + 5" class="star empty">☆</span>
                </div>
                <h3 class="testimonial-name">{{ testimonial.name }}</h3>
                <p class="testimonial-role">{{ testimonial.role }}</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script>
  import { testimonials } from "@/assets/data/testimonials";
  
  export default {
    name: "TestimonialSection",
    data() {
      return {
        testimonials,
      };
    },
  };
  </script>
  
  <style scoped>
  .testimonial-section {
    padding: 4rem 2rem;
    background-color: #f9f9f9;
    text-align: center;
    font-family: 'Epilogue', sans-serif;

  }
  
  .section-title {
    font-size: 2rem;
    margin-bottom: 2rem;
    color: #333;
  }
  
  .testimonials-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr); 
    gap: 2rem;
  }
  
  .testimonial-card {
    background: #fff;
    padding: 1.5rem;
    border: 1px solid #ddd;
    border-radius: 10px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    display: flex;
    flex-direction: column;
    align-items: flex-start;
  }
  
  .testimonial-quote {
    font-style: italic;
    font-size: 1rem;
    font-weight: 700;
    color: #555;
    margin-bottom: 1.5rem;
    text-align: left;
  }
  
  .testimonial-card-footer {
    display: flex;
    align-items: center;
    gap: 1.5rem;
    width: 100%;
  }
  
  .testimonial-image {
    width: 80px;
    height: 80px;
    border-radius: 50%;
    object-fit: cover;
    border: 2px solid #ddd;
  }
  
  .testimonial-text {
    text-align: left;
    flex: 1;
  }

  .testimonial-name,
  .testimonial-rating {
    font-family: 'Epilogue', sans-serif;
    font-size: 1.2rem;
    color: #000; 
    margin-bottom: 0.5rem;
  }
  
  .star.empty {
    color: #ddd;
  }
  
  .testimonial-name {
    font-weight: bold;
    font-size: 1.1rem;
    margin-bottom: 0.3rem;
    color: #333;
  }
  
  .testimonial-role {
    font-size: 0.9rem;
    color: #777;
  }

  .section-title {
    font-size: 2rem;
    font-weight: 700;
    text-align: center;
    margin-bottom: 2rem;
    color: #333;
  } 
  </style>
  