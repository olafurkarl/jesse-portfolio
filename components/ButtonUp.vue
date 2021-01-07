<template>
  <a v-smooth-scroll href="#top" class="button_circle">
    <i class="fa fa-angle-up" />
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
  background-color: #1A3163;
  bottom: 0;
  border-radius: 4.5px;
  display: flex;
  align-items: center;
  position: fixed;
  top: 50%;
  right: 1%;
  text-decoration: none;
}

i {
  color: white;
  font-size: 20px;

  margin-left: auto;
  margin-right: auto;
}
</style>
