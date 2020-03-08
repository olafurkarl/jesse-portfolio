<template>
  <div class="topbar">
    <div class="name">
      <span>Jesse Ting</span> <span>(Jian Yu)</span>
    </div>
    <div class="navigation">
      <a class="topbar-work">Work</a>
      <a class="topbar-about">About</a>
      <a class="topbar-contact">Contact</a>
    </div>
  </div>
</template>

<style scoped>

.topbar {
  display: grid;
  grid-template-columns: 2.8fr 1.7fr;
  grid-template-rows: 1fr;
  grid-template-areas:
  "name navigation";
  width: 100%;
  height: 104px;
  left: 0px;
  top: 0px;

  align-items: center;
}

@media(max-width: 375px) {
  .topbar {
    grid-template-columns: 1fr;
    grid-template-rows: 1fr;
    grid-template-areas:
    "name";
  }

  .topbar-work, .topbar-about, .topbar-contact {
    display: none;
  }

  .name {
      justify-self: center;
  }
}

.name { grid-area: name; }

.empty { grid-area: empty; }

.navigation { grid-area: navigation; }

.padding-right { grid-area: padding-right; }

.padding-left { grid-area: padding-left; }

.name {
  font-family: Montserrat;
  font-style: normal;
  font-weight: bold;
  font-size: 22px;
  line-height: 27px;

  color: #607D8B;
}

.navigation {
  text-align: right;
  float: right;

  font-family: Montserrat;
  font-style: normal;
  font-weight: bold;
  font-size: 22px;
  line-height: 27px;

  color: #607D8B;

  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 1fr;
  grid-template-areas: ". . .";
  grid-area: navigation;
}

</style>
