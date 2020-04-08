<template>
  <div>
    <div class="challenges">
      <div class="challenge">
        <img src="~assets/design_challenge/001.png">
      </div>
      <div class="challenge">
        <img src="~assets/design_challenge/002.png">
      </div>
      <div class="challenge">
        <img src="~assets/design_challenge/003.png">
      </div>
      <div class="challenge">
        <img src="~assets/design_challenge/004.png">
      </div>
      <div class="challenge">
        <img src="~assets/design_challenge/005.png">
      </div>
      <div class="challenge">
        <img src="~assets/design_challenge/006.png">
      </div>
      <div class="challenge">
        <img src="~assets/design_challenge/007.png">
      </div>
      <div class="challenge last">
        <img src="~assets/design_challenge/008.png">
      </div>
    </div>
  </div>
</template>

<style>
.challenges {
  display: block;
  max-width: 1050px;
  margin: auto;

  grid-template-rows: repeat(auto-fill, minmax(0, 1fr));

  padding-top: 4em;
}

.challenge {
  margin-bottom: 4em;
}

.last {
  margin-bottom: 13em;
}

@media (max-width: 1200px) {
  .challenge img {
    width: 100%;
    object-fit: sclae-down;
  }
};

</style>
