<template>
  <div class="galleryImages">
    <img src="../assets/shop/store.jpg" alt="store of items" />
    <img src="../assets/shop/set.jpg" alt="set of items" />
    <img src="../assets/shop/dogrug.jpg" alt="dog on a rug" />
    <img src="../assets/shop/board.jpg" alt="pin board" />
    <img src="../assets/shop/sheep.jpg" alt="sheep cushion" />
    <img src="../assets/shop/hunting.jpg" alt="hunting cushion" />
    <img src="../assets/shop/farm.jpg" alt="farm cushion" />
    <img src="../assets/shop/horse.jpg" alt="horse cushion" />
  </div>
</template>

<style scoped>
.galleryImages {
  display: inline-grid;
  grid-template-columns: repeat(4, 1fr);
  grid-gap: 5em;
  width: 100%;
  padding: 0 10em;
}

img {
  display: flex;
  justify-content: center;
  align-items: center;
  box-shadow: 0 6px 8px rgba(0, 0, 0, 0.4);
  margin: 0 auto;
}

@media (max-width: 1024px) {
  .galleryImages {
    grid-template-columns: repeat(2, 1fr);
    padding: 0 1em;
  }
}

@media (max-width: 600px) {
  .galleryImages {
    grid-template-columns: 1fr 1fr;
    padding: 1em;
    grid-gap: 2em;
  }
}
</style>
