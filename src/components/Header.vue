<template>
    <header class="header">
      <div class="container">
    
        <div class="header-content">
          <div class="logo">LOGO</div>
          <nav>
            <ul class="nav-links">
              <li><a href="#about">About</a></li>
              <li><a href="#work">Work</a></li>
              <li><a href="#contact">Contact</a></li>
            </ul>
          </nav>
        </div>
  
        
        <div class="header-new-content">
          <div class="header-left">
            <p class="subheading">Branding | Image making</p>
            <h1 class="main-heading">Visual Designer</h1>
            <p class="description">
              This is a template Figma file, turned into code using Anima. <br />
              Learn more at AnimaApp.com
            </p>
            <button class="contact-btn">Contact</button>
          </div>
          <div class="header-right">
            <div class="image-container">
              <img src="@/assets/HeaderImage.png" alt="Visual Designer" />
              <div class="decorative-shapes">
                <div class="shape red"></div>
                <div class="shape green"></div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </header>
  </template>
  
  <style scoped>

  .header {
    background-color: #fff;
    padding: 1rem 0;
    border-bottom: 1px solid #ddd;
  }
  
  .header-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  
  .logo {
    font-size: 1.5rem;
    font-weight: 700;
  }
  
  .nav-links {
    list-style: none;
    display: flex;
    gap: 2rem;
    margin: 0;
    padding: 0;
  }
  
  .nav-links a {
    font-weight: 600;
    color: #000;
    text-transform: uppercase;
    font-size: 0.9rem;
    transition: color 0.2s;
  }
  
  .nav-links a:hover {
    color: #333;
  }
  
  
  .header-new-content {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-top: 2rem;
  }
  
  .header-left {
    max-width: 50%;
  }
  
  .subheading {
    font-size: 1.2rem;
    font-weight: 600;
    color: #333;
    margin-bottom: 1rem;
  }
  
  .main-heading {
    font-size: 3rem;
    font-weight: 700;
    margin-bottom: 1rem;
    color: #000;
  }
  
  .description {
    font-size: 1rem;
    line-height: 1.5;
    margin-bottom: 2rem;
    color: #555;
  }
  
  .contact-btn {
    padding: 0.8rem 1.5rem;
    background-color: #000;
    color: #fff;
    border: none;
    font-size: 1rem;
    font-weight: 600;
    height: 60px;
    width: 170px;
    cursor: pointer;
    transition: background-color 0.3s;
  }
  
  .contact-btn:hover {
    background-color: #333;
  }
  
  .header-right {
    position: relative;
    max-width: 40%;
  }
  
  .image-container {
    position: relative;
    display: inline-block;
  }
  
  .image-container img {
    max-width: 100%;
    border-radius: 20px;
  }
  
  .decorative-shapes .shape {
    position: absolute;
    width: 50px;
    height: 50px;
    border-radius: 10px;
  }
  
  .shape.red {
    background-color: #ff6f61;
    top: -10%;
    right: -10%;
  }
  
  .shape.green {
    background-color: #00897b;
    bottom: -10%;
    left: -10%;
  }
  </style>
  