<template>
  <div>
    <div class="container">
      <div class="content grey">
        <div class="padding-left" />
        <div class="padding-right" />
        <TopBar />
      </div>
      <div class="content">
        <div class="padding-left" />
        <div class="padding-right" />
        <MainHeader />
      </div>
      <div id="projects" />
      <div class="content projects">
        <div class="padding-left" />
        <div class="padding-right" />
        <Projects />
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
import TopBar from '~/components/TopBar.vue'
import MainHeader from '~/components/MainHeader.vue'
import Projects from '~/components/Projects.vue'
import Footer from '~/components/Footer.vue'

export default {
  components: {
    TopBar,
    MainHeader,
    Projects,
    Footer
  },
  head () {
    return {
      title: 'Jesse\'s Portfolio',
      meta: [
        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        { hid: 'og:title', content: 'Jesse Ting\'s Portfolio.' },
        { hid: 'og:image', content: '/preview.jpg' },
        { hid: 'og:url', content: 'https://.jesseding.now.sh' }
      ]
    }
  }
}
</script>

<style>
.grey {
  background-color: #F5F5F5;
}

#projects {
  padding: 0.8em;
}

.projects {
  background-color: #F7F7F7;
}

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
