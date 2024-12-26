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
</style>
