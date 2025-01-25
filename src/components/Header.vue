<template>
  <h1>WILDLY QUACKERS</h1>
  <div class="header-links">
    <a href="/">HOME</a>
    <a href="">SHOP</a>
    <a href="/">CONTACT</a>
  </div>
</template>

<style scoped>
h1 {
  font-size: 2.5rem;
  text-align: center;
  padding: 20px;
  font-family: lora;
  font-weight: 600;
  letter-spacing: 5px;
  text-decoration: underline;
  text-decoration-color: rgb(50, 143, 75);
  text-decoration-thickness: 2px;
  text-underline-offset: 20px;
  padding-bottom: 40px;
}

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

@media (max-width: 768px) {
  h1 {
    font-size: 1.8rem; /* Scale down the font size */
    padding: 15px; /* Adjust padding for better alignment */
    text-underline-offset: 10px; /* Adjust underline offset for smaller text */
    padding-bottom: 30px;
  }
}
</style>
