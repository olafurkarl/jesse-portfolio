<template>
  <div>
    <div class="container">
      <div class="content grey">
        <div class="padding-left" />
        <div class="padding-right" />
        <TopBar />
      </div>
      <ButtonUp />
      <div class="content main">
        <div class="padding-left" />
        <div class="padding-right" />
        <div class="center">
          <div v-if="loggedIn">
            <div class="padded">
              <IntroHeader title="Vai Vu - Conferencing App" left="UX/UI Case Study" right="October - December 2020" />
              <div class="imageCentered">
                <img src="~/assets/vai/vai1.png">
              </div>
              <Summary>
                Vai Vu is a conferencing application that enables users to have face-to-face meetings with collaborative features,
                such as Miro Board, screen sharing, and annotations. The scope of this project includes reskinning an existing conferencing app,
                Jitsi, to align it with the Vai product family, supporting several third party integrations (Miro, Slack, ClickUp),
                and optimising the experience of hosting and scheduling a meeting from Arena, the platfrom that hosts meetings for the customers.
              </Summary>

              <br>
              <Hashtags>
                #User Experience  &nbsp; #Product Design &nbsp;  #Branding  &nbsp; #Telecommunication
              </Hashtags>
              <br>
              <br>
              <div class="imageCentered">
                <img src="~/assets/vai/vai2.png">
              </div>

              <YellowCard title="Discover" number="01.">
                After the kick off meeting with the product team and multiple conversations with the lead developer,
                I got a fair understanding of the vision scope in this project and the current implementation of the product, Vai Vu.
                <br>
                <br>
                One of the biggests problems we were facing was the lack of design consistency across the
                two platforms which causes a disjointed product experience. In addition, the current user flows for the most common tasks needed to be investigated and optimised.

                <br>
                <br>
                I used Miro to map out every primary user flow in order to see the whole picture.
                Then I started identifying the prominent issues and forming hypotheses. These hypotheses were then tested for validation.
              </YellowCard>
              <div class="imageCentered">
                <img src="~/assets/vai/vai3.png">
              </div>
              <br>
              <br>
              <br>
              <br>
              <YellowCard title="Research" number="02.">
                As the project touched three different platforms, I listed the research tasks under each platform to clarify the targeted problems,
                and I conducted a series of competitor analyses in order to find the best solution that tackles each listed issue.
              </YellowCard>
              <div class="imageCentered">
                <img src="~/assets/vai/vai4.png">
                <img src="~/assets/vai/vai5.png">
              </div>

              <p>
                For Jitsi’s information architecture issue, I conducted a Card Sorting session with a colleague from the customer
                support team since he has the least experience with the app.
                From that, it helped me to find where the pain points are and restructure the feature layout as well as the navigation.
              </p>

              <div class="imageCentered">
                <img src="~/assets/vai/vai6.png">
              </div>
              <YellowCard title="Ideate & Test" number="03.">
                I sketched out a couple of potential solutions that could improve the experience relating to the identified issues and tested them with the product team.
              </YellowCard>

              <div class="imageCentered">
                <img src="~/assets/vai/vai7.png">
              </div>
              <p>
                I also reconstructed the entire user flow starting from Arena’s login, to leaving the meeting room,
                and had several meetings with the lead developer to discuss the technical feasibility.
              </p>
              <div class="imageCentered">
                <img src="~/assets/vai/vai8.png">
              </div>
              <p>
                From the card sorting session, I found the themes that would help group certain features together and placed them in more accessible and logical locations.
                The features are grouped by whether they’re client-side or affect the meeting itself (on the top left side and on the right side respectively).
                The mini screen on the bottom should allow the users to interact with individual participants; however, it also allows users to close it to increase the
                visibility of the meeting.
              </p>

              <div class="imageCentered">
                <img src="~/assets/vai/vai9.png">
              </div>

              <YellowCard title="Prototype" number="04.">
                Once the new user flow and sketches had been reviewed, I transformed each approved paper wireframe into Hi-fi prototypes on Figma,
                and started designing the transition effects on different screens.
              </YellowCard>

              <div class="imageCentered">
                <img src="~/assets/vai/vai10.png">
              </div>

              <div class="imageCentered">
                <img src="~/assets/vai/vai11.png">
              </div>

              <div class="imageCentered">
                <img src="~/assets/vai/vai12.png">
              </div>

              <div class="imageCentered">
                <img src="~/assets/vai/vai13.png">
              </div>

              <YellowCard title="Handoff" number="05.">
                This project consists of redesigning an existing product, Arena, and reshaping a template, Jitsi. To complete a smooth handoff,
                I not only delivered Hi-fi prototypes on Figma but I also created style guides for both products. For Jitsi, which is now Vai Vu,
                was an easier task; However, it was not easy to create the proper a style guide for Arena as it was built without a design systematic approach.
                Every component is built on top of one another. Thus, listing out the component inventory was really crucial as well as specifically instructing the
                dev team which components we were replacing from the new design.
              </YellowCard>

              <div class="imageCentered">
                <img src="~/assets/vai/vai14.png">
              </div>
            </div>
            <ThankYou />
          </div>
          <div v-else>
            <PasswordPrompt />
          </div>
        </div>
      </div>
      <br>
      <Footer />
    </div>
  </div>
</template>

<script>
import IntroHeader from '~/components/IntroHeader.vue'
import Hashtags from '~/components/Hashtags.vue'
import YellowCard from '~/components/YellowCard.vue'
import ThankYou from '~/components/ThankYou.vue'
import PasswordPrompt from '~/components/PasswordPrompt.vue'

export default {
  components: {
    IntroHeader,
    Hashtags,
    YellowCard,
    ThankYou,
    PasswordPrompt
  },
  computed: {
    loggedIn () {
      return this.$store.state.login.loggedIn
    }
  }
}
</script>

<style scoped>
p {
  font-family: Karla;
  font-style: normal;
  font-weight: normal;
  font-size: 20px;
  line-height: 30px;
}

.content.main {
  min-height: 1400px;
}

.imageCentered img {
  max-width: 100%;
}

.imageCentered {
    text-align: center;
    margin-bottom: 3em;
    margin-top: 3em;
}

@media (max-width: 1200px) {
  .imageCentered img {
    width: 100%;
    object-fit: scale-down;
  }
};
</style>
