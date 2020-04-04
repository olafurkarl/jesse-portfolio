<template>
  <div class="blue-title">
    {{ title }}
  </div>
</template>

<style scoped>
.blue-title {
  font-family: Montserrat;
  color: #1A3163;
  font-weight: 600;
  font-size: 36px;

  justify-content: left;

  margin-bottom: 1em;
  margin-top: 5px;
}
</style>

<script>
export default {
  props: {
    title: { type: String, default: 'Title' }
  }
}
</script>
