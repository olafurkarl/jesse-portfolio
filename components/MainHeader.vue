<template>
  <div class="grid-container">
    <div class="text">
      <div class="hello">
        Hello
      </div>
      <div class="introduction">
        I'm Jesse Ting
      </div>
      <div class="description">
        <div>a UX/UI designer</div>
        <br>
        <div>based in Brisbane</div>
        <br>
        <div>Australia</div>
      </div>
    </div>
    <div class="image">
      <img src="~assets/jesse_main.png">
    </div>
    <div class="button">
      <ButtonDown />
    </div>
  </div>
</template>

<style scoped>
@keyframes slideInFromLeft {
  0% {
    transform: translateX(-200%);
  }
  100% {
    transform: translateX(0);
  }
}

@keyframes fadeIn {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}

.grid-container {
  display: grid;
  grid-template-columns: minmax(0, 1fr);
  grid-template-rows: [text] 1.8fr;
  grid-template-areas:
  "text"
  "image"
  "button";

  margin-bottom: 35px;
  justify-items: center;
  text-align: center;
  justify-content: space-between;
}

@media(min-width: 1100px) {
  .grid-container {
    display: grid;
    grid-template-columns: auto auto;
    grid-template-rows: [text] 1.8fr;
    grid-template-areas:
    "text image"
    "text image"
    "button button";
    text-align: left;
  }
}

.image {
  grid-area: image;
  overflow: hidden;
 }

.text {
  grid-area: text;
  width: 100%;
  word-wrap: break-word;
  overflow-wrap: break-word;
 }

.button { grid-area: button; }

.image {
  grid-area: image;
  text-align: right;
}

.text { grid-area: text; }

.button {
    grid-area: button;
    grid-column-start: button;
    grid-column-end: span 2;
    justify-self: center;
}

img {
  width: 561px;
  height: 671px;

  animation: 1.3s ease-in-out 0s 1 fadeIn;

  overflow: hidden;
  object-fit: cover;
  max-width: 100%;
}

.text {
  font-family: Montserrat;
  font-style: normal;
  font-weight: normal;
  font-size: 70px;
  line-height: 85px;
  display: block;
  align-self: center;
  animation: 0.5s ease-in-out 0s 1 slideInFromLeft;
}

@media(max-width: 700px) {
  .text {
    font-size: 30px;
    margin-top: 50px;
  }
}

.hello {
  color: #E35975;
}

.description {
  font-weight: bold;
}

.description > div {
  padding-inline-end: 10px;
  padding-inline-start: 10px;
  display: inline-block;
  background: linear-gradient(to top, transparent 30%, #0AE6B4 30% 65%, transparent 35%);
  white-space: nowrap;
}
</style>

<script>
import ButtonDown from '~/components/ButtonDown.vue'

export default {
  components: {
    ButtonDown
  }
}
</script>
