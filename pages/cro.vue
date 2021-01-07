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
        <div class="center">
          <div class="padded">
            <IntroHeader title="CRO + UI Redesign" left="UI Redesign Showcase" right="January - April 2020" />
            <Summary>
              CRO (Conversion Rate Optimisation) is the process of enhancing your digital products to boost conversions,
              which means to convert a website visitor into a paying customer.
              This showcase demonstrates my understanding of the problems solved by CRO techniques,
              coupled with practicing quick ideation sessions to come up with potential solutions to be tested,
              putting an emphasis on design consistency.
            </Summary>

            <div class="grey-box">
              <h2>01. Nespresso</h2>
              <p>
                <b>Problem Statement:</b>
                There is a missed opportunity on Nespresso website to present relevant products to users more easily and engagingly
                and motivate them to purchase (Current implementation below).
              </p>
              <CroImages image1="nespresso1.png" image2="nespresso1-hor.png" />
              <p>
                <b>Proposed Solutions:</b>
                Present customers with filtering options on homepage / link to Guided Selling
                to help them quickly find the right product (Proposed designs below).
              </p>
              <p>
                Variation 1: Intensity filter
              </p>
              <CroImages image1="nespresso2.png" image2="nespresso3-hor.png" has-shadow />
              <CroImages image1="nespresso3.png" image2="nespresso3-hor.png" has-shadow />
              <p>
                Variation 2: Cup Sizes
              </p>
              <CroImages image1="nespresso4.png" image2="nespresso4-hor.png" has-shadow />
              <CroImages image1="nespresso5.png" image2="nespresso5-hor.png" has-shadow />
            </div>
            <div class="grey-box">
              <h2>02. Shine Lawyers</h2>
              <p>
                <b>Problem Statement:</b>
                When searching for a claim, a list of random assortments of content is displayed in the list below.
                This means when users are searching for a claim,
                a list of random assortments of content is displayed in the list below (Current implementation below).
              </p>
              <CroImages image1="shine1.png" image2="shine1-hor.png" />
              <p>
                <b>Proposed Solutions:</b>
                The objective of this round is to determine the best way to order search results so customers can quickly and easily find what they want (Proposed designs below).
              </p>
              <p>
                Step 1 - Enter search words
              </p>
              <CroImages image1="shine2.png" image2="shine2-hor.png" has-shadow />
              <p>
                Step 2 - Select filter by xxx
              </p>
              <p>
                Filtered by "Order"
              </p>
              <CroImages image1="shine3.png" image2="shine3-hor.png" has-shadow />
              <p>
                Filtered by "Legal"
              </p>
              <CroImages image1="shine4.png" image2="shine4-hor.png" has-shadow />
              <p>
                Filtered by "Location"
              </p>
              <CroImages image1="shine5.png" image2="shine5-hor.png" has-shadow />
            </div>

            <div class="grey-box">
              <h2>03. CV Check</h2>
              <p>
                <b>Problem Statement:</b>
                The UI of the check ordering process is out of date and can cause user anxiety and lack of trust in CVCheck
                (Current implementation below)
              </p>
              <img class="single-image" src="~/assets/cro/cv1.png">
              <p>
                <b>Proposed Solutions:</b>
                Redesign the UI and visual design of the ordering process while maintaining the design consistency (Proposed design below).
              </p>
              <img class="single-image" src="~/assets/cro/cv2.png">
              <img class="single-image" src="~/assets/cro/cv3.png">
            </div>
          </div>
        </div>
      </div>
      <br>
      <Footer />
    </div>
  </div>
</template>

<script>
import TopBar from '~/components/TopBar.vue'
import Footer from '~/components/Footer.vue'
import ButtonUp from '~/components/ButtonUp.vue'
import IntroHeader from '~/components/IntroHeader.vue'
import Summary from '~/components/Summary.vue'
import CroImages from '~/components/CroImages.vue'

export default {
  components: {
    TopBar,
    Footer,
    ButtonUp,
    IntroHeader,
    Summary,
    CroImages
  }
}
</script>

<style scoped>

p {
  font-size: 20px;
  line-height: 29px;
  margin-bottom: 2em;
}

.single-image {
  margin-bottom: 2em;
}

.grey-box > img {
  object-fit: cover;
  width: 100%;
  padding-left: 2%;
  padding-right: 2%;
}

.grey-box > h2 {
  font-family: Karla;
  font-style: normal;
  font-weight: bold;
  font-size: 36px;
  line-height: 29px;
  color: #1A3163;
  padding-top: 1em;
  padding-bottom: 1em;
}

.grey-box {
  margin-top: 2em;
  text-align: left;
  background-color: rgba(221, 221, 221, 0.3);
  padding: 0px 4em 0em 4em;
}
</style>
