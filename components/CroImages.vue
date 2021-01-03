<template>
  <div class="imageContainer">
    <div class="imageGrid">
      <img :src="require(`~/assets/cro/${image1}`)" width="600px">
      <img :src="require(`~/assets/cro/${image2}`)" width="200px">
    </div>
  </div>
</template>

<style scoped>

</style>

<style scoped>
.imageContainer {
    display: block;
    max-width: 1050px;
    padding-bottom: 2em;
}

.imageGrid {
    display: grid;
    justify-content: space-evenly;
    grid-template-columns: 1fr 1fr;
    column-gap: 5%;
    object-fit: scale-down;
}

/* @media (max-width: 1200px) {
  .imageContainer img {
    width: 100%;
    object-fit: scale-down;
  }
}; */
</style>

<script>
export default {
  props: {
    image1: { type: String, default: '' },
    image2: { type: String, default: '' }
  }
}
</script>
