<template>
  <div>
    <div class="container">
      <div class="content grey">
        <div class="padding-left" />
        <div class="padding-right" />
        <TopBar />
      </div>
      <ButtonUp />
      <div class="content">
        <div class="padding-left" />
        <div class="padding-right" />
        <div class="">
          <div class="main-description padded">
            <div class="description-text">
              <img src="~assets/myfootcare-part-one/qut-2.png">

              <div class="grey-header-small">
                <div class="grey-header-left">
                  UX/UI Case Study
                </div>
                <div class="grey-header-right">
                  February - October 2019
                </div>
              </div>
              <div class="text">
                MyFootCare (MFC) Thermal is a health app that aims to assist Diabetic Foot Ulcer (DFU) patients in self-managing  their individual recovering condition by measuring the size and temperature of their ulcers captured by taken pictures either by themselves or with the  assistance of home carers. With the enhancement of the thermal image camera Flir One, users can understand the stage of their wounds more accurately to decrease the possibility of facing the terminal stages of the disease.
              </div>
              <br>
              <br>
              <div class="hashtags">
                #User Experience &nbsp;  #Usability Testing &nbsp; #Healthcare &nbsp; #User Interview
              </div>
            </div>
          </div>
          <br>
          <br>
          <br>
          <br>
          <div class="scope padded">
            <BlueHeader title="Scope" />
            <div class="text">
              01. Prototype and test solutions with participants.
            </div>
            <br>
            <div class="text">
              02. Conduct compatibility testing (Flir One and Android system in mobile devices)
            </div>

            <img src="~assets/myfootcare-part-two/scope.png">
          </div>
          <div class="break" />
          <div class="empathy padded">
            <GreyDivider />

            <BlueHeader title="Empathy" />

            <div class="text">
              Based on the research of DFU and collected insights from usability testing and interviews, I created two Personas to illustrate the needs, behaviours, and goals of my users. This approach allowed me to see clearly which tasks (and in which contexts) would help MFC users use the app with satisfaction.
            </div>
          </div>

          <img src="~assets/myfootcare-part-two/empathy.png" class="empathy-img">

          <div class="break" />

          <div class="user-flow padded">
            <GreyDivider />

            <BlueHeader title="User Flow" />

            <div class="text">
              Once the pain points were discovered, I created a user flow and mapped out the stages where users had trouble proceed. According to the UX research, the senior demographic was the target audience. Creating a simple workflow and having a clean user interface would improve the user experience and learnability.
            </div>

            <img src="~assets/myfootcare-part-two/mcs-flow-chart.png">
          </div>

          <div class="break" />

          <div class="prototype padded">
            <GreyDivider />

            <BlueHeader title="Prototype" />

            <div class="text">
              With the framework of the new user flow, a series of low-fidelity sketches were made, not only to visually illustrate the potential solutions of each pain points but also ensured identified issues were validated by asking feedback from participants. By doing so, it helped to refine the design solutions and effectively reshape the new Hi-fidelity prototype.
            </div>

            <img src="~assets/myfootcare-part-two/low-fi-mcs.png">

            <div class="text">
              To clearly see the entire process with created low fidelity sketch features, I created a mid-fidelity wireframe with user flow. Using this approach, I could more efficiently and accurately understand the user’s journey with new changes. I also removed unnecessary tasks in the process flow.
            </div>

            <img src="~assets/myfootcare-part-two/user-flow-and-wireframe.png">

            <div class="text">
              The second part of the foot check-up was a series of area segmentation of the foot image to help the algorithm capture the size of the wound accurately. This part of the user flow was augmented by implementing animations instead of graphics to teach users how to perform the area segmentation.
            </div>
          </div>

          <div class="break" />

          <div class="hifi-prototype padded">
            <GreyDivider />

            <BlueHeader title="Hi-Fi Prototype" />

            <div class="text">
              <b>Design Recommedation 1</b> | NEW HOME SCREEN <br>
              To improve learnability and understanding of the app, a new home screen was made.
            </div>

            <img src="~assets/myfootcare-part-two/comparison.png">

            <div class="text">
              <b>Design Recommedation 2</b> | NEW SETTING PAGE <br>
              Before a lot of important features were hidden in the inconspicuous ‘More’ section which included Settings and Notifications. The suggested improvement was creating a new Settings page and recategorizing the features to improve navigability.
            </div>

            <img src="~assets/myfootcare-part-two/comparison2.png">

            <div class="text">
              <b>Design Recommedation 3</b> | ANIMATE PICTURE SEGMENTATION <br>
              GUIDANCE
              Animation of the instructions improveed the image segmentation performed by the users after temperature check-ups. This new design had not only made the user flow smoother but also increased memorability.
            </div>

            <img src="~assets/myfootcare-part-two/comparison3.png">
          </div>

          <div class="break" />

          <div class="validate padded">
            <GreyDivider />

            <BlueHeader title="Validate" />

            <div class="text">
              Each sketch and wireframe was reviewed with the participants iteratively before moving on to the next stage. With user feedback, a Hi-Fi prototype was developed through Sketch. As none of my participant had a DFU condition, I decided to validate my proposed design recommendations with a friend of mine who actually has  diabetes type 1.
            </div>

            <img src="~assets/myfootcare-part-two/ratings-and-reviews.png" style="max-width: 369px;">
          </div>

          <div class="quote">
            <br>
            Steve Krug stated in his book DON'T MAKE ME THINK - "Testing one user is 100% better than testing none"
            <br>
            <br>
          </div>

          <div class="padded">
            <img src="~assets/myfootcare-part-two/style-guide.png">
          </div>

          <div class="break" />

          <div class="delivery padded">
            <GreyDivider />

            <BlueHeader title="Delivery" />

            <div class="text">
              Two design sprints were planned to work with the development collaboratively. The first part of the design was to investigate the user experience of the application and the integration of the thermal image camera FLIR ONE. The second part focused more on optimising the user experience design in terms of navigability, learnability, and usability by redesigning the identified problem on the user interface. The outcome of the design and research enabled this project to meet the expectation which was to assist DFU patients and promote a self-care approach in healthcare practice.
            </div>
          </div>
        </div>

        <div class="outro padded">
          UX Research part of this case study can be found in the <nuxt-link to="/myfootcare-part-one">
            Part 1
          </nuxt-link>
        </div>

        <ThankYou />
      </div>

      <Footer />
    </div>
  </div>
</template>

<script>
import TopBar from '~/components/TopBar.vue'
import ThankYou from '~/components/ThankYou.vue'
import BlueHeader from '~/components/BlueHeader.vue'
import GreyDivider from '~/components/GreyDivider.vue'
import Footer from '~/components/Footer.vue'
import ButtonUp from '~/components/ButtonUp.vue'

export default {
  components: {
    TopBar,
    ThankYou,
    BlueHeader,
    GreyDivider,
    Footer,
    ButtonUp
  }
}
</script>

<style scoped>
.text + img {
  margin-bottom: 5em;
}

@media (max-width: 420px) {
  .text + img {
    margin-bottom: 2em;
  }
}

.grey {
  background-color: #F5F5F5;
}

.quote::before {
  content: '';
  border-top: 2px solid #dddddd;
  width: 40%;
  left: 30%;
  position: absolute;
}

.quote::after {
  content: '';
  border-bottom: 2px solid #dddddd;
  width: 40%;
  left: 30%;
  position: absolute;
}

.quote {
  font-family: Montserrat;
  color: #1A3163;
  font-weight: 600;
  font-size: 36px;
  line-height: 40px;
  text-align: center;
  margin-top: 2em;
  margin-bottom: 2em;
}

.padding-right { grid-area: padding-right; }

.padding-left { grid-area: padding-left; }

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

.grey-header-right {
  margin-left: auto;
}

.description-text > img {
  width: 100%;
  object-fit: cover;
}

.text {
  font-family: Karla;
  font-size: 20px;
  line-height: 30px;
}

.hashtags {
  font-family: Karla;
  font-size: 20px;
}

.scope img {
  margin-top: 2.5em;
}

img {
  width: 100%;
  object-fit: cover;

  margin-top: 5em;
}

.main-description img {
  margin-top: 0em;
}

.empathy-img {
  text-align: center;
  max-width: 1050px;
  display: block;
  margin: auto;
  margin-top: 3em;
}

.questions {
  margin-top: 1em;
  font-family: Karla;
  font-style: normal;
  font-weight: normal;
  font-size: 25px;
  line-height: 29px;
  align-items: center;
}

.synthesis img {
  margin-top: 3em;
}

.recommendations img {
  max-width: 391px;
  margin-top: 2em;
}

.outro {
  font-family: Montserrat;
  font-style: normal;
  font-weight: 500;
  font-size: 30px;
  line-height: 37px;
  align-items: center;
  text-align: center;
  color: #1A3163;
  margin-top: 3em;
  margin-bottom: 2em;
}

@media(max-width: 420px) {
  .outro {
    font-size: 24px;
  }
}

.outro a {
  text-decoration-line: underline;
  color: #F26582;
}

</style>
