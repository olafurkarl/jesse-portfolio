<template>
  <div id="top" class="topbar">
    <div class="name">
      <nuxt-link to="/about" class="topbar-about nostyle">
        <span>Jesse Ting</span> <span>(Jian Yu)</span>
      </nuxt-link>
    </div>
    <div class="navigation">
      <nuxt-link to="/" class="topbar-about nostyle">
        Home
      </nuxt-link>
      <nuxt-link to="/about" class="topbar-about nostyle">
        About
      </nuxt-link>
      <nuxt-link v-smooth-scroll :to="{ path: '/',hash:'#projects'}" href="#projects" class="topbar-about nostyle">
        Projects
      </nuxt-link>
      <a href="https://medium.com/@jcding" class="topbar-about nostyle">
        Blog
      </a>
    </div>
  </div>
</template>

<style scoped>

.topbar {
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

  .name {
    display: block;
  }

  .navigation {
    display: none !important;
  }

  .navigation a {
    display: none;
    grid-column-gap: 0em;
  }

  .name {
      justify-self: center;
  }
}

.name { grid-area: name; }

.empty { grid-area: empty; }

.navigation { grid-area: navigation; }

.name {
  font-family: Montserrat;
  font-style: normal;
  font-weight: 600;
  font-size: 22px;
  line-height: 27px;

  color: #1A3163;
}

.navigation {
  text-align: right;
  float: right;

  font-family: Montserrat;
  font-style: normal;
  font-weight: 600;
  font-size: 22px;
  line-height: 27px;

  color: #1A3163;

  display: grid;
  grid-template-columns: fit-content(100%) fit-content(100%) fit-content(100%) fit-content(100%);
  grid-template-rows: 1fr;
  grid-template-areas: ". . .";
  grid-area: navigation;

  justify-self: self-end;

  grid-column-gap: 2em;
  white-space: nowrap;
}

.navigation a {
  grid-column-gap: 2em;
  text-decoration: none;
  color: #1A3163;
}

.topbar a {
  text-decoration: none;
  color: #1A3163;
}

.nuxt-link-exact-active, .nuxt-link-active {
  text-decoration: none;
  color: #1A3163;
}
</style>
