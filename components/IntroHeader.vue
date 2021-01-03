<template>
  <div class="main-description">
    <div class="description-text">
      <h1 class="intro-header">
        {{ title }}
      </h1>
      <div class="grey-header-small">
        <div class="grey-header-left">
          {{ left }}
        </div>
        <div class="grey-header-right">
          {{ right }}
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: { type: String, default: 'Title' },
    left: { type: String, default: 'Left' },
    right: { type: String, default: 'Right' }
  }
}

</script>

<style scoped>
.main-description {
  margin-top: 5em;
}

.intro-header {
  font-family: Montserrat;
  font-style: normal;
  text-align: left;
  font-weight: 500;
  font-size: 48px;
  line-height: 58px;
  color: #1A3163;
}

@media(max-width: 420px) {
  .main-description {
    margin-top: 1em;
  }
}

.description-text > img {
  width: 100%;
  object-fit: cover;
}

.grey-header-right {
  margin-left: auto;
}

.grey-header-small {
  font-family: Karla;
  font-style: normal;
  font-weight: 300;
  font-size: 20px;
  line-height: 58px;

  display: flex;
  align-items: center;

  color: #666666;

  border-top: 1px solid #DDDDDD;

  margin-top: 1em;
}

@media (max-width: 420px) {
  .grey-header-small {
    font-size: 12px;
    line-height: 32px;
  }
}
</style>
