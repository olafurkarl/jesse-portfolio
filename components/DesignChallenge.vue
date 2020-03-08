<template>
  <div>
    <div class="title">
      UI Daily Design Challenge
    </div>
    <div class="challenges">
      <div class="design-challenge-2">
        <img src="~assets/design_challenge/design-challenge-1-1.png" data-aos="flip-right">
        <img src="~assets/design_challenge/design-challenge-1-2.png" data-aos="flip-left">
      </div>

      <div class="design-challenge-2">
        <img src="~assets/design_challenge/design-challenge-2-1.png" data-aos="flip-right">
        <img src="~assets/design_challenge/design-challenge-2-2.png" data-aos="flip-left">
      </div>

      <div class="design-challenge-2">
        <img src="~assets/design_challenge/design-challenge-3-1.png" data-aos="flip-right">
        <img src="~assets/design_challenge/design-challenge-3-2.png" data-aos="flip-left">
      </div>

      <div class="design-challenge-3">
        <img src="~assets/design_challenge/design-challenge-4-1.png" data-aos="flip-right">
        <img src="~assets/design_challenge/design-challenge-4-2.png" data-aos="flip-up">
        <img src="~assets/design_challenge/design-challenge-4-3.png" data-aos="flip-left">
      </div>

      <div class="design-challenge-2">
        <img src="~assets/design_challenge/design-challenge-5-1.png" data-aos="flip-right">
        <img src="~assets/design_challenge/design-challenge-5-2.png" data-aos="flip-left">
      </div>
    </div>
  </div>
</template>

<style>
.title {
  grid-area: projects-title;
  font-family: Montserrat;
  font-style: normal;
  font-weight: normal;
  font-size: 60px;
  line-height: 73px;
  display: flex;
  justify-self: center;
  justify-content: center;

  color: #E35975;

  margin-top: -0.6em;
}

.challenges {
  display: grid;
  margin-bottom: 20px;
  grid-row-gap: 2em;

  max-width: 100vw;
}

.design-challenge-2 {
  display: grid;
  grid-template-columns: auto;
  grid-template-rows: auto auto;
  justify-content: space-evenly;
  align-items: center;
}

.design-challenge-3 {
  display: grid;
  grid-template-columns: auto;
  grid-template-rows: auto auto auto;

  justify-content: space-evenly;
  align-items: center;
}

@media(max-width: 950px) {
  .title {
    font-size: 6vw;
    position: absolute;
    margin-top: -4vh;
  }

  .challenges {
    padding-top: 7vh;
  }
}

@media(max-width: 1150px) {
  .challenges > div {
    max-width: 40vw
  }
  .challenges > div > img {
    justify-self: center;
    object-fit: scale-down;
    max-width: 80vw;
    margin-bottom: 10px;
  }
  .challenges {
    justify-content: space-evenly;
  }
}

@media(min-width: 1150px) {
  .design-challenge-2 {
    display: grid;
    grid-template-columns: auto auto;
    justify-content: space-evenly;
    align-items: center;
  }

  .design-challenge-3 {
    display: grid;
    grid-template-columns: auto auto auto;
    justify-content: space-evenly;
    align-items: center;
  }
}

</style>
