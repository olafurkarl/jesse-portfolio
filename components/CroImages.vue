<template>
  <div class="imageContainer">
    <div class="imageGrid">
      <img :src="require(`~/assets/cro/${image1}`)" :class="{ shadow: hasShadow }">
      <img :src="require(`~/assets/cro/${image2}`)" :class="{ shadow: hasShadow }">
    </div>
  </div>
</template>

<script>
export default {
  props: {
    image1: { type: String, default: '' },
    image2: { type: String, default: '' },
    hasShadow: { type: Boolean, default: false }
  }
}
</script>

<style scoped>
.imageContainer {
    display: block;
    max-width: 1050px;
    padding-bottom: 2em;
}

.shadow {
  box-shadow: 0px 8px 24px 0px rgba(0, 0, 0, 0.2);
}

.imageGrid {
    display: grid;
    justify-content: space-evenly;
    grid-template-columns: 1fr 1fr;
    column-gap: 5%;
}

@media (max-width: 1200px) {
  .imageGrid {
    display: grid;
    justify-content: space-evenly;
    grid-template-columns: 40%;
    grid-template-rows: repeat(auto-fill, minmax(0, 1fr));
    grid-column-gap: 5%;
    grid-row-gap: 5%;
    text-align: center;
    -o-object-fit: scale-down;
    object-fit: scale-down;
    margin-bottom: 3em;
  }

  img {
    justify-self: center;
    -o-object-fit: scale-down;
    object-fit: scale-down;
    width: 100%;
  }
};
</style>
