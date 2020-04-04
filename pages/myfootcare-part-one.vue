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
        <div class="">
          <div class="main-description padded">
            <div class="description-text">
              <img src="~assets/myfootcare-part-one/qut-1.png">

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
              01. Evaluate the current design development through UX research
            </div>
            <br>
            <div class="text">
              02. Document the uncover user problems for future assessment
            </div>

            <img src="~assets/myfootcare-part-one/scope.png">
          </div>
          <div class="break" />
          <div class="research padded">
            <GreyDivider />

            <BlueHeader title="Research" />

            <div class="text">
              Initially, I looked into some health information regarding DFU on diabetic related websites to understand the treatment process and the symptoms of the disease, I also had regular meetings with my supervisor and the product owner in order to understand the project background and requirements.
            </div>

            <br>

            <div class="text">
              It was understood that DFU self-management through mobile applications was an ongoing research project which started 6 years ago, so there were not sufficient competitors to compare directly. Most outcomes of the development and testing were presented through academic papers. In addition, the integration of a thermal image camera with a health app in this area was mostly in the testing phase.
            </div>
          </div>

          <img src="~assets/myfootcare-part-one/companies.png" class="companies-img">

          <div class="break" />

          <div class="design-review padded">
            <GreyDivider />

            <BlueHeader title="Design Review" />

            <div class="text">
              As the product was at the beta testing phase and had not launched on the market, gaining user feedback was limited, and reviewing user interviews and user interface designs became crucial to get a deeper understanding of the project.
            </div>

            <img src="~assets/myfootcare-part-one/design-review-pictures.png">
          </div>

          <div class="break" />

          <div class="usability-testing padded">
            <GreyDivider />

            <BlueHeader title="Usability Testing" />

            <div class="text">
              5 participants were invited to take part of this research though none of them actually has experienced Diabetic Foot Ulcers (DFU). Due to an ethic approval requirement at QUT for engaging in this type of research with targeted users, this project was not permitted to conduct interviews and tests with actual DFU patients during the project time. Thus, the requirement of test candidates was merely having a basic understanding of using a smartphone and being capable of taking a picture. A screen recorder was on to capture everything during each testing.
            </div>

            <img src="~assets/myfootcare-part-one/foot-pictures.png">
          </div>

          <div class="break" />

          <div class="user-interview padded">
            <GreyDivider />

            <BlueHeader title="User Interview" />

            <div class="text">
              A interview guide was create to assist the facilitation of user interviews. The goal was to understand the pain point of their experience and how they feel about the design.
            </div>

            <div class="questions">
              <div>
                01. Overall, how would you describe your experience with the application?
              </div>
              <br>
              <div>
                02. Was it what you expected? Did anything surprise you?
              </div>
              <br>
              <div>
                03. Was taking the foot check overall easy or difficult to understand?
              </div>
              <br>
              <div>
                04. Were the previous foot check records easy or difficult to find?
              </div>
              <br>
              <div>
                05. If you could change one or more thing from what you’ve seen today,  what would it be?
              </div>
              <br>
              <div>
                06. Imagine you had DFU, would you use this app?
              </div>
            </div>
          </div>

          <div class="break" />

          <div class="synthesis padded">
            <GreyDivider />

            <BlueHeader title="Synthesis" />

            <div class="text">
              I prioritised which issues were more important to solve by listing the spent time of each testing from long to short and labelling each proposed problem with participant’s name. Later on, I used an affinity mapping approach to find connections and patterns. Multiple complaints about the long spent time were regarded as high priority. Less frequency and less time consumption are less urgent at the preliminary stage.
            </div>

            <img src="~assets/myfootcare-part-one/jesse-stickies.png">
            <img src="~assets/myfootcare-part-one/swot.png">
          </div>

          <div class="break" />

          <div class="recommendations padded">
            <GreyDivider />

            <BlueHeader title="Recommendations" />

            <div class="text">
              SWOT analysis was conducted to create feasible design recommendations based on the results of affinity mapping. However, it was not practical to implement every finding in the design changes. I concentrated on 3 features that would optimize user experience.
            </div>

            <img src="~assets/myfootcare-part-one/recommendations.png">
          </div>
        </div>

        <div class="outro padded">
            UI Design &amp; Delivery part of this case study can be found in <nuxt-link to="/myfootcare-part-two">Part 2</nuxt-link>
          </div>

        <ThankYou />
      </div>
    </div>
  </div>
</template>

<script>
import TopBar from '~/components/TopBar.vue'
import ThankYou from '~/components/ThankYou.vue'
import BlueHeader from '~/components/BlueHeader.vue'
import GreyDivider from '~/components/GreyDivider.vue'

export default {
  components: {
    TopBar,
    ThankYou,
    BlueHeader,
    GreyDivider
  }
}
</script>

<style scoped>
.padded {
  margin-left: 20%;
  margin-right: 20%;
}

.break {
  padding-bottom: 6em;
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

.grey-header-small {
  font-family: Karla;
  font-style: normal;
  font-weight: 300;
  font-size: 20px;
  line-height: 58px;

  display: flex;
  align-items: center;

  color: #666666;

  border: none;
}

.grey-header-right {
  margin-left: auto;
}

.description-text {
  margin-top: 108px;
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
}

.companies-img {
  text-align: center;
  max-width: 1000px;
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
}

.outro a {
  text-decoration-line: underline;
  color: #1A3163;
}

</style>
