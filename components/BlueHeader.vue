<template>
  <div class="blue-title">
    {{ title }}
  </div>
</template>

<script>
export default {
  props: {
    title: { type: String, default: 'Title' }
  }
}
</script>

<style scoped>
.blue-title {
  font-family: Montserrat;
  color: #1A3163;
  font-weight: 600;
  font-size: 36px;

  justify-content: left;

  margin-bottom: 1em;
  margin-top: 30px;
}

@media (max-width: 420px) {
  .blue-title {
    font-size: 24px;
    text-align:  center;
  }
}
</style>
