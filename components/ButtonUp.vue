<template>
  <a v-smooth-scroll href="#top" class="button_circle">
    <i class="las la-angle-up" />
  </a>
</template>

<script>
export default {
  methods: {
    scrollToTop () {
      window.scrollTo(0, 0)
    }
  }
}
</script>

<style scoped>
.button_circle {
  width: 25px;
  height: 25px;

  background-color: #F7F7F7;
  bottom: 0;

  border-radius: 12.5px;

  display: flex;
  align-items: center;

  position: fixed;

  border: 2px solid #FFFFFF;

  top: 50%;
  right: 1%;

  text-decoration: none;
}

i {
  color: #999999;
  font-weight: bold;
  font-size: 16px;

  margin-left: auto;
  margin-right: auto;
}
</style>
