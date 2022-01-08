<template>
  <div class="grid-container">
    <div class="projects-title">
      Projects
    </div>

    <!-- <div class="box-5">
      <nuxt-link to="/vai">
        <img class="image box-5-image" src="~assets/box-5.png">
      </nuxt-link>
    </div> -->
    <div class="box-1">
      <nuxt-link to="/cro">
        <img class="image box-6-image" src="~assets/box-6.png">
      </nuxt-link>
    </div>
    <div class="box-2">
      <nuxt-link to="/flight-centre">
        <img class="image box-1-image" src="~assets/box-1.png">
      </nuxt-link>
    </div>
    <div class="box-3">
      <nuxt-link to="/design-challenge">
        <img class="image box-4-image" src="~assets/box-design-challenge.png">
      </nuxt-link>
    </div>
    <div class="box-4">
      <nuxt-link to="/myfootcare-part-one">
        <img class="image box-2-image" src="~assets/box-qut-1.png">
      </nuxt-link>
    </div>
    <div class="box-5">
      <nuxt-link to="/myfootcare-part-two">
        <img class="image box-3-image" src="~assets/box-qut-2.png">
      </nuxt-link>
    </div>
  </div>
</template>

<style scoped>

a:link {
    text-decoration: inherit;
    color: inherit;
}

a:visited {
    text-decoration: inherit;
    color: inherit;
}

.grid-container {
  display: grid;
  grid-template-columns: auto auto auto;
  grid-template-rows: 0.3fr 2.5fr 2.5fr;
  grid-template-areas:
  "projects-title projects-title projects-title"
  "box-1 box-2 box-3"
  "box-4 box-5 box-6";
  align-content: center;
  justify-content: center;
  justify-items: center;
  grid-gap: 4em;

  margin-bottom: 4em;
}

@media (max-width: 420px) {
  .grid-container {
    grid-gap: 1em;
  }
}
.padding-left { grid-area: padding-left; }

.padding-right { grid-area: padding-right; }

.projects-title {
  grid-area: projects-title;
  font-family: Montserrat;
  font-style: normal;
  font-weight: normal;
  font-size: 60px;
  line-height: 73px;
  justify-self: center;

  color: #E35975;

  margin-top: -0.6em;
  text-align: center;
}

.padding-bottom { grid-area: padding-bottom; }

.text {
  font-family: Montserrat;
  font-style: normal;
  font-weight: bold;
  font-size: 20px;
  line-height: 24px;
  margin-top: 16px;
  margin-bottom: 16px;
  width: 280px;
}

.image {
  display: block;
  width: 100%;
  max-width: 280px;
}

.box-1 {
  display: inline-grid;
  grid-template-columns: 1fr;
  grid-template-rows: auto auto;
  grid-template-areas: "box-1-image" "box-1-text";
  grid-area: box-1;
  justify-self: center;
  text-align: center;
}

.box-1-text { grid-area: box-1-text; }

.box-2 {
  display: inline-grid;
  grid-template-columns: 1fr;
  grid-template-rows: auto auto;
  grid-template-areas: "box-2-image" "box-2-text";
  grid-area: box-2;
  justify-self: center;
}

.box-2-text { grid-area: box-2-text; }

.box-3 {
  display: inline-grid;
  grid-template-columns: 1fr;
  grid-template-rows: auto auto;
  grid-template-areas: "box-3-image" "box-3-text";
  grid-area: box-3;
  justify-self: center;
}

.box-3-text { grid-area: box-3-text; }

.box-4 {
  display: inline-grid;
  grid-template-columns: 1fr;
  grid-template-rows: auto auto;
  grid-template-areas: "box-4-image" "box-4-text";
  grid-area: box-4;
  justify-self: center;
}

.box-5 {
  display: inline-grid;
  grid-template-columns: 1fr;
  grid-template-rows: auto auto;
  grid-template-areas: "box-5-image" "box-5-text";
  grid-area: box-5;
  justify-self: center;
}

.box-6 {
  display: inline-grid;
  grid-template-columns: 1fr;
  grid-template-rows: auto auto;
  grid-template-areas: "box-6-image" "box-6-text";
  grid-area: box-6;
  justify-self: center;
}

.box-4-text { grid-area: box-4-text; }
</style>
