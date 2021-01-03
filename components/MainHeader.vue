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
        <div>A UX Designer</div>
        <br>
        <div>based in Sydney</div>
        <br>
        <div>Australia</div>
      </div>
    </div>
    <div class="image">
      <img src="~assets/jesse_main.png">
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

  margin-top: 6em;
  margin-bottom: 6em;
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
  align-self: center;
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
  animation: 1.3s ease-in-out 0s 1 fadeIn;

  max-width: 516px;
  max-height: 530px;
  width: 100%;
  object-fit: scale-down;
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
  padding-right: 10px;
}

@media(max-width: 420px) {
  .grid-container {
    margin-top: 1em;
  }

  .text {
    font-size: 30px;
    line-height: 40px;
    margin-bottom: 1em;
  }
}

.hello {
  color: #E35975;
}

.description {
  font-weight: 600;
}

.description > div {
  padding-inline-end: 10px;
  padding-inline-start: 10px;
  display: inline-block;
  background: linear-gradient(to top, transparent 30%, #0AE6B4 30% 50%, transparent 50%);
  white-space: nowrap;
}
</style>
