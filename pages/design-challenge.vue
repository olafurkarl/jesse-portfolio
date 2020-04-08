<template>
  <div>
    <div class="container">
      <div class="content grey">
        <div class="padding-left" />
        <div class="padding-right" />
        <TopBar />
      </div>
      <ButtonUp />
      <div class="title">
        UI Daily Design Challenge
      </div>
      <div class="text">
        I started UI design challenges by designing various themes of user interface and components to improve my UI skills
      </div>
      <div class="content challenges-main">
        <div class="padding-left" />
        <div class="padding-right" />
        <div class="center">
          <DesignChallenge />
        </div>
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
import Footer from '~/components/Footer.vue'
import TopBar from '~/components/TopBar.vue'
import DesignChallenge from '~/components/DesignChallenge.vue'
import ButtonUp from '~/components/ButtonUp.vue'

export default {
  components: {
    TopBar,
    Footer,
    DesignChallenge,
    ButtonUp
  }
}
</script>

<style scoped>
.challenges-main {
  background-color: #F7F7F7;
  text-align: center;
  margin-top: 4em;
}

.title {
  grid-area: projects-title;
  font-family: Montserrat;
  font-style: normal;
  font-weight: normal;
  font-size: 60px;
  line-height: 73px;
  text-align: center;

  color: #E35975;

  margin-top: 1em;
}

.text {
  font-family: Montserrat;
  font-style: normal;
  font-weight: 500;
  font-size: 20px;
  line-height: 24px;
  align-items: center;
  text-align: center;

  color: #000000;

  margin-top: 1em;
  margin-bottom: 1em;
}
</style>
