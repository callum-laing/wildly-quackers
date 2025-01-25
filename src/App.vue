<script setup>
import { ref } from 'vue'
import Header from './components/Header.vue'
import Hero from './components/Hero.vue'
import Discover from './components/Discover.vue'
import Products from './components/Products.vue'
import Contact from './components/Contact.vue'
import Footer from './components/Footer.vue'

const heroSection = ref(null)
const productsSection = ref(null)
const contactSection = ref(null)

const scrollToSection = (section) => {
  if (section === 'home') {
    window.scrollTo({ top: 0, behavior: 'smooth' })
  } else if (section === 'shop') {
    productsSection.value.scrollIntoView({ behavior: 'smooth' })
  } else if (section === 'contact') {
    contactSection.value.scrollIntoView({ behavior: 'smooth' })
  }
}
</script>

<template>
  <main>
    <Header />
    <div class="header-links">
      <a href="#" @click.prevent="scrollToSection('home')">HOME</a>
      <a href="#" @click.prevent="scrollToSection('shop')">SHOP</a>
      <a href="#" @click.prevent="scrollToSection('contact')">CONTACT</a>
    </div>

    <div ref="heroSection">
      <Hero />
    </div>

    <h2>Discover the Heart of Artisan Crafting</h2>
    <Discover />

    <h2>Featured Products</h2>
    <div ref="productsSection">
      <Products />
    </div>

    <h2>
      Artisan home decor inspired by nature's finest materials with designs by Delphine Brooks, Sam
      Bowker-Laing and others
    </h2>
    <div ref="contactSection">
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
