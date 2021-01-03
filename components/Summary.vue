<template>
  <div>
    <h3>Summary</h3>
    <div class="text">
      <slot />
    </div>
  </div>
</template>

<style scoped>
h3 {
  font-family: Karla;
  font-style: normal;
  font-weight: bold;
  font-size: 20px;
  line-height: 29px;

  margin-top: 30px;
}

.text {
  font-family: Karla;
  font-style: normal;
  font-weight: normal;
  font-size: 20px;
  line-height: 30px;
  margin-top: 20px;

  display: flex;
  align-items: center;
}

</style>
