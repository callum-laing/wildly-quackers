<script setup>
import Header from './components/Header.vue'
import Hero from './components/Hero.vue'
import Discover from './components/Discover.vue'
import Products from './components/Products.vue'
import Contact from './components/Contact.vue'
import Footer from './components/Footer.vue'
</script>

<template>
  <main>
    <Header />
    <nav class="header-links">
      <a href="#shop">SHOP</a>
      <a href="#contact">CONTACT</a>
    </nav>

    <Hero />

    <h2>Discover the Heart of Artisan Crafting</h2>
    <Discover />

    <h2 id="shop">Featured Products</h2>
    <Products />

    <h2>
      Artisan home decor inspired by nature's finest materials with designs by Delphine Brooks, Sam
      Bowker-Laing and others
    </h2>
    <div id="contact">
      <Contact />
    </div>
    <Footer />
  </main>
</template>

<style scoped>
.header-links {
  text-align: center;
}

.header-links > a {
  text-decoration: none;
  margin: 0 20px;
  color: black;
  letter-spacing: 2px;
}

.header-links > a:hover {
  color: rgb(50, 143, 75);
}

h2 {
  font-size: 4rem;
  text-align: center;
  padding: 50px 0;
  font-family: yellowtail;
  color: green;
}

@media (max-width: 768px) {
  h2 {
    font-size: 2rem;
    padding: 30px 10px;
  }
}
</style>
