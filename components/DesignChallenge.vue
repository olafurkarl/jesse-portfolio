<template>
  <div class="grid-container">
    <div class="title">
      UI Daily Design Challenge
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

  color: #E35975;

  margin-top: -0.6em;
}

.grid-container {
  display: grid;
  grid-template-columns: auto;
  grid-template-rows: 0.3fr 2.5fr 2.5fr 2.5fr 2.5fr;
  grid-template-areas:
  "projects-title"
  "box-1"
  "box-2"
  "box-3"
  "box-4";

  text-align: center;
  align-content: space-between;
  justify-content: space-between;
}

@media(max-width: 700px) {
  .grid-container {
      align-content: center;
      justify-content: center;
  }
}

@media (min-width: 700px) {
  .grid-container {
    grid-template-columns: auto auto;
    grid-template-rows: 0.3fr 2.5fr 2.5fr;
    grid-template-areas:
    "projects-title projects-title"
    "box-1 box-2"
    "box-3 box-4";
  }
}

@media (min-width: 1200px) {
  .grid-container {
    grid-template-columns: auto auto auto auto;
    grid-template-rows: 0.3fr 2.5fr;
    grid-template-areas:
    "projects-title projects-title projects-title projects-title"
    "               box-1 box-2 box-3 box-4                     "
  }
}
</style>
