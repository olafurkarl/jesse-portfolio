<template>
  <div class="topbar">
    <div class="name">
      <span>Jesse Ting</span> <span>(Jian Yu)</span>
    </div>
    <div class="navigation">
      <nuxt-link to="/">
        <a class="topbar-home">Home</a>
      </nuxt-link>
      <nuxt-link to="/">
        <a class="topbar-work">About</a>
      </nuxt-link>
      <nuxt-link to="/">
        <a class="topbar-about">Projects</a>
      </nuxt-link>
      <nuxt-link to="/">
        <a class="topbar-contact">Daily UI</a>
      </nuxt-link>
    </div>
  </div>
</template>

<style scoped>

.topbar {
  background-color: #F5F5F5;
  display: grid;
  grid-template-columns: 1fr 3fr;
  grid-template-rows: 1fr;
  grid-template-areas:
  "name navigation";
  width: 100%;
  height: 104px;
  left: 0px;
  top: 0px;

  align-items: center;
}

@media(max-width: 750px) {
  .topbar {
    grid-template-columns: 1fr;
    grid-template-rows: 1fr;
    grid-template-areas:
    "name";
  }

  .navigation a {
    display: none;
    grid-column-gap: 0;
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
  grid-template-columns: 1fr 1fr 1fr 1fr;
  grid-template-rows: 1fr;
  grid-template-areas: ". . .";
  grid-area: navigation;

  justify-self: self-end;
}

.navigation a {
  padding-left: 1em;
  grid-column-gap: 2em;
}

.nuxt-link-exact-active, .nuxt-link-active {
  text-decoration: none;
  color: #607D8B;
}

</style>
