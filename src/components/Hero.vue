<template>
  <div class="hero">
    <div class="card">
      <img src="../assets/dog2.png" alt="dog on a bed" />
    </div>
  </div>
</template>

<style scoped>
.hero {
  margin-top: 50px;
  min-height: 75dvh;
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
  box-shadow: 0 6px 8px rgba(0, 0, 0, 0.4);
  padding: 20px;
  width: 800px;
  text-align: center;
  margin-bottom: -80px;
  padding-top: 100px;
}

.card img {
  width: 100%;
  margin-bottom: 100px;
}

@media (max-width: 768px) {
  .hero {
    margin-top: 20px;
    min-height: 60dvh;
    background-size: cover; /* Scale background to fit */
    padding: 10px;
  }

  .card {
    width: 90%; /* Adjust card width for smaller screens */
    padding: 15px;
    margin-bottom: -50px; /* Reduce margin for smaller view */
    padding-top: 80px;
  }

  .card img {
    margin-bottom: 50px; /* Reduce image bottom margin */
  }
}
</style>
