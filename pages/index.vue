<template>
  <div>
    <div class="container">
      <div class="content">
        <div class="padding-left" />
        <div class="padding-right" />
        <TopBar />
      </div>
      <div class="content">
        <div class="padding-left" />
        <div class="padding-right" />
        <MainHeader />
      </div>
      <div class="content">
        <div class="padding-left" />
        <div class="padding-right" />
        <Projects />
      </div>
      <div class="content">
        <div class="empty" />
      </div>
      <div class="content">
        <div class="padding-left" />
        <div class="padding-right" />
        <DesignChallenge />
      </div>
    </div>
  </div>
</template>

<script>
import TopBar from '~/components/TopBar.vue'
import MainHeader from '~/components/MainHeader.vue'
import Projects from '~/components/Projects.vue'
import DesignChallenge from '~/components/DesignChallenge.vue'

export default {
  components: {
    TopBar,
    MainHeader,
    Projects,
    DesignChallenge
  }
}
</script>

<style>
.content {
  display: grid;
  grid-template-columns: 0.1fr minmax(0, 1fr) 0.1fr;
  grid-template-rows: auto auto auto auto;
  grid-template-areas:
  "padding-left content-1 padding-right"
  "padding-left content-2 padding-right"
  "padding-left content-3 padding-right"
  "padding-left content-4 padding-right";

  justify-content: center;
}

.empty {
  height: 10em;
}

.content:nth-of-type(odd) {
  background: #F5F5F5;
}

.container-1 {
    grid-column-start: padding-left;
    grid-column-end: padding-right;
    background: #F5F5F5;
}

.navigation { grid-area: navigation; }

.padding-right { grid-area: padding-right; }

.padding-left { grid-area: padding-left; }

</style>
