<template>
  <div>
    <div class="title">
      UI Daily Design Challenge
    </div>
    <div class="challenges">
      <!-- <div class="challenges-2">
        <img class="design-challenge" src="~assets/design_challenge/design-challenge-1-1.png">
        <img class="design-challenge" src="~assets/design_challenge/design-challenge-1-2.png">
      </div>
      <div class="challenges-2">
        <img class="design-challenge" src="~assets/design_challenge/design-challenge-2-1.png">
        <img class="design-challenge" src="~assets/design_challenge/design-challenge-2-2.png">
      </div>
      <div />
      <div class="challenges-2">
        <img class="design-challenge" src="~assets/design_challenge/design-challenge-3-1.png">
        <img class="design-challenge" src="~assets/design_challenge/design-challenge-3-2.png">
      </div>
      <div />
      <div class="challenges-3">
        <img class="design-challenge" src="~assets/design_challenge/design-challenge-4-1.png">
        <img class="design-challenge" src="~assets/design_challenge/design-challenge-4-2.png">
        <img class="design-challenge" src="~assets/design_challenge/design-challenge-4-3.png">
      </div>
      <div />
      <div />
      <div class="challenges-2">
        <img class="design-challenge" src="~assets/design_challenge/design-challenge-5-1.png">
        <img class="design-challenge" src="~assets/design_challenge/design-challenge-5-2.png">
      </div>
    </div> -->
      <img class="design-challenge" src="~assets/design_challenge/design-challenge-1-1.png">
      <img class="design-challenge" src="~assets/design_challenge/design-challenge-1-2.png">

      <img class="design-challenge" src="~assets/design_challenge/design-challenge-2-1.png">
      <img class="design-challenge" src="~assets/design_challenge/design-challenge-2-2.png">

      <img class="design-challenge" src="~assets/design_challenge/design-challenge-3-1.png">
      <img class="design-challenge" src="~assets/design_challenge/design-challenge-3-2.png">

      <img class="design-challenge" src="~assets/design_challenge/design-challenge-4-1.png">
      <img class="design-challenge" src="~assets/design_challenge/design-challenge-4-2.png">
      <img class="design-challenge" src="~assets/design_challenge/design-challenge-4-3.png">

      <img class="design-challenge" src="~assets/design_challenge/design-challenge-5-1.png">
      <img class="design-challenge" src="~assets/design_challenge/design-challenge-5-2.png">
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
  justify-content: space-evenly;
  margin-bottom: 20px;
  grid-template-columns: repeat(auto-fit, 1fr);
}

/* .challenges-2 {
  grid-template-columns: auto auto;
}

.challenges-3 {
  grid-template-columns: auto auto auto;
} */

.design-challenge {
  object-fit: cover;
}
</style>
