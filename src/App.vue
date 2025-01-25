<script setup>
import Header from './components/Header.vue'
import Hero from './components/Hero.vue'
import Discover from './components/Discover.vue'
import Products from './components/Products.vue'
import Contact from './components/Contact.vue'
</script>

<template>
  <main>
    <Header />
    <Hero />
    <h2>Discover the Heart of Artisan Crafting</h2>
    <Discover />
    <h2>Featured Products</h2>
    <Products />
    <h2>
      Artisan home decor inspired by nature's finest materials with designs by Delphine Brooks, Sam
      Bowker-Laing and others
    </h2>
    <Contact />
  </main>
</template>

<style scoped>
h2 {
  font-size: 4rem;
  text-align: center;
  padding: 50px 0;
  font-family: yellowtail;
  color: green;
}

@media (max-width: 768px) {
  h2 {
    font-size: 2rem; /* Reduce font size for smaller screens */
    padding: 30px 10px; /* Adjust padding for better spacing */
  }
}
</style>
