<template>
  <div id="app">
    <Header />
    <main class="main-content">
      <h1>Welcome</h1>
      <p>To be countined.</p>
    </main>
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Footer,
  },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Epilogue:wght@400;600;700&display=swap');

body {
  font-family: 'Epilogue', sans-serif;
  margin: 0;
  padding: 0;
  color: #000;
  background-color: #fff;
  box-sizing: border-box;
}

#app {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

.main-content {
  flex: 1;
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 2rem;
}

.main-content h1 {
  font-size: 2.5rem;
  font-weight: 700;
  margin-bottom: 1rem;
}

.main-content p {
  font-size: 1.2rem;
  color: #333;
}
</style>
