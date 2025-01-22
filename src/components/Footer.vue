<template>
    <footer class="footer">
      <div class="footer-container">
    
        <div class="footer-left">
          <h2>Let's work together</h2>
          <p>
            This is a template Figma file, turned into code using Anima. Learn
            more at AnimaApp.com. This is a template Figma file, turned into code
            using Anima. Learn more at AnimaApp.com
          </p>
          <div class="social-icons">
            <a href="https://discord.com" target="_blank">
              <img src="@/assets/discord.png" alt="Discord" />
            </a>
            <a href="https://facebook.com" target="_blank">
              <img src="@/assets/facebook.png" alt="Facebook" />
            </a>
            <a href="https://dribbble.com" target="_blank">
              <img src="@/assets/dribbble.png" alt="Dribbble" />
            </a>
            <a href="https://instagram.com" target="_blank">
              <img src="@/assets/instagram.png" alt="Instagram" />
            </a>
            <a href="https://behance.net" target="_blank">
              <img src="@/assets/behance.png" alt="Behance" />
            </a>
          </div>
        </div>
  
        
        <div class="footer-right">
          <form class="contact-form">
            <div class="form-fields">
              <label for="name">Name</label>
              <input type="text" id="name" placeholder="Your Name" />
  
              <label for="email">Email</label>
              <input type="email" id="email" placeholder="Your Email" />
            </div>
            <div class="form-button">
              <button type="submit">Submit</button>
            </div>
          </form>
        </div>
      </div>
    </footer>
  </template>
  
  <style scoped>
  .footer {
    background-color: #f5f5f5;
    padding: 2rem 0;
    width: 100%;
  }
  
  .footer-container {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    max-width: 1200px;
    margin: 0 auto;
    gap: 2rem;
    flex-wrap: wrap;
  }
  
  .footer-left {
    flex: 1;
  }
  
  .footer-left h2 {
    font-size: 1.5rem;
    font-weight: 700;
    margin-bottom: 1rem;
  }
  
  .footer-left p {
    color: #333;
    margin-bottom: 1.5rem;
  }
  
  .social-icons {
    display: flex;
    gap: 1rem;
  }
  
  .social-icons img {
    width: 40px;
    height: 40px;
    transition: transform 0.2s ease;
  }
  
  .social-icons img:hover {
    transform: scale(1.1);
  }
  
  .footer-right {
    flex: 1;
  }
  
  .contact-form {
    display: flex;
    flex-direction: column;
    gap: 1.5rem;
  }
  
  .form-fields {
    display: flex;
    flex-direction: column;
    gap: 1rem;
  }
  
  .contact-form label {
    font-weight: 600;
    font-size: 1rem;
  }
  
  .contact-form input {
    padding: 0.8rem;
    border: 1px solid #ccc;
    border-radius: 4px;
    width: 100%;
    box-sizing: border-box;
  }
  
  .contact-form input:focus {
    outline: none;
    border-color: #000;
  }
  
  .form-button {
    text-align: left;
  }
  
  .contact-form button {
    background-color: #000;
    color: #fff;
    padding: 0.7rem;
    font-weight: 600;
    height: 60px;
    border: none;
    width: 200px;
    cursor: pointer;
    transition: background-color 0.3s ease;
  }
  
  .contact-form button:hover {
    background-color: #333;
  }
  </style>
  