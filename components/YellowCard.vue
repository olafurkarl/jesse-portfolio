<template>
  <div>
    <div class="card-number">
      {{ number }}
    </div>
    <div class="card-info">
      <div class="card-title">
        {{ title }}
      </div>
      <div class="card-text">
        <slot />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: { type: String, default: 'Title' },
    number: { type: String, default: '00.' }
  }
}
</script>

<style scoped>
.card-number {
  font-family: Montserrat;
  font-style: normal;
  font-weight: normal;
  font-size: 85px;

  display: flex;
  align-items: center;

  color: #F9BA5D;
}

.card-title {
  font-family: Montserrat;
  font-style: normal;
  font-weight: 600;
  font-size: 29px;
  line-height: 29px;

  margin-bottom: 1em;
}

.card-text, .card-text-2 {
  font-family: Karla;
  font-style: normal;
  font-weight: normal;
  font-size: 20px;
  line-height: 30px;
}
</style>
