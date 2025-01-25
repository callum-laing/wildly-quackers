<template>
  <div class="discover">
    <div class="discover-img">
      <img src="../assets/cushions.png" alt="" />
    </div>
    <div class="discover-text">
      <h3>OUR UNIQUE PROCESS</h3>
      <p>
        At Wildly Quackers, we take pride in our meticulously crafted items made from the
        by-products of animals such as hide, wool, and sheepskin. Our commitment to sustainability
        ensures that each piece tells a story while being environmentally friendly.
      </p>
    </div>
  </div>
</template>

<style scoped>
.discover {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 100px;
}

.discover-text {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  gap: 20px;
}

.discover-text h3 {
  font-size: 1.3rem;
  letter-spacing: 2px;
  font-weight: bold;
}

.discover-text p {
  font-size: 1.2em;
  line-height: 1.75;
  max-width: 400px;
}

img {
  width: 600px;
  height: auto;
  padding: 20px;
}

@media (max-width: 768px) {
  .discover {
    flex-direction: column;
    gap: 40px;
    padding: 20px;
  }

  .discover-text p {
    font-size: 1rem;
    max-width: 100%;
  }
}
</style>
