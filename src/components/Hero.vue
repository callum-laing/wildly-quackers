<template>
  <div class="hero">
    <div class="card">
      <img src="../assets/dogs.jpg" alt="Two dogs on a bed" />
    </div>
  </div>
  <div>
    <h2>Discover the Heart of Artisan Crafting</h2>
  </div>
</template>

<style scoped>
.hero {
  margin-top: 50px;
  min-height: 50dvh;
  background-image: url(../assets/wild.png);
  background-size: 90%;
  background-repeat: no-repeat;
  background-position: center;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 20px;
  box-sizing: border-box;
  position: relative;
}

.card {
  background-color: white;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
  padding: 20px;
  max-width: 400px;
  text-align: center;
}

.card img {
  width: 100%;
  border-radius: 10px;
  margin-bottom: 10px;
}

h2 {
  font-size: 3rem;
  text-align: center;
}
</style>
