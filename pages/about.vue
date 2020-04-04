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
        <div class="center">
          <div class="about-intro">
            <img src="~assets/about/jesse-sunglasses.png">

            <div class="greeting-text">
              I'm <span class="name">Jesse Ting</span>, a UX/UI designer based in Brisbane Australia
            </div>
          </div>

          <div class="side-grey-line">
            <h3>About Me</h3>
            <div class="text">
              Born and raised in Taipei Taiwan with a passion in crafting physical and digital products. Recently graduated from QUT with a master of IT in user experience track. While I was completing my study, I interned in Flight Centre HQ working with the Retail Experience Team and worked as a freelance UX consultant. Design Thinking process, for me, is a mindset that helps human to solve problem in an innovative and creative approach which is critical to what I do and believe.
            </div>
          </div>

          <div class="side-by-side">
            <div class="side-grey-line">
              <h3>Education</h3>
              <ul>
                <li>
                  <div class="cv-header">
                    Queensland University of Technology
                  </div>
                  <div class="cv-text">
                    Master of IT - User Expereince track
                  </div>
                  <div class="cv-footer">
                    Feb 2018 - Dec 2019 | Brisbane, Australia
                  </div>
                </li>
                <li>
                  <div class="cv-header">
                    Tamkang University
                  </div>
                  <div class="cv-text">
                    Bachelor of Arts - English Language and Culture
                  </div>
                  <div class="cv-footer">
                    Sep 2011 - Jun 2015 | Ilan, Taiwan
                  </div>
                </li>
                <li>
                  <div class="cv-header">
                    Temple University
                  </div>
                  <div class="cv-text">
                    Global Exchange Program
                  </div>
                  <div class="cv-footer">
                    Jul 2013 - Jun 2014 | Philadelphia, USA
                  </div>
                </li>
              </ul>
            </div>

            <div class="side-grey-line">
              <h3>Specialties</h3>
              <div class="text">
                <ul>
                  <li>
                    UX Research
                  </li>
                  <li>Product Design</li>
                  <li>Interaction Design</li>
                  <li>Prototyping </li>
                  <li>Usability Testing</li>
                  <li>Problem Solving</li>
                  <li>Wireframing</li>
                  <li>Business Process Mgt</li>
                  <li>Heuristic Review</li>
                </ul>
              </div>
            </div>
          </div>

          <div class="side-grey-line">
            <div class="cv-item">
              <div class="cv-header">
                Junior UX/UI Designer / Conversions King
              </div>
              <div class="cv-footer">
                Jan 2020 - Mar 2020 | Brisbane, Australia
              </div>
              <ul>
                <li>
                  Ensured the delivery of consistent and logical user experience – derived from customer insights and UX knowledge.
                </li>
                <li>
                  Drafted and refined user flows, wireframes, prototypes, design and testing to take my design from concept through to the final product, with support from the Head of Product and the design team.
                </li>
              </ul>
            </div>

            <div class="cv-item">
              <div class="cv-header">
                UX/UI Design Intern / Flight Centre Travel Group
              </div>
              <div class="cv-footer">
                Jul 2019 - Oct 2019 | Brisbane, Australia
              </div>
              <ul>
                <li>
                  Assisted Retail Experience team, got involved with everything from
                  design sprints to design execution.
                </li>
                <li>
                  Designed email templates for internal use between customer support managers and national travel consultants.
                </li>
                <li>
                  Researched current digital design system guidelines and practices.
                </li>
              </ul>
            </div>

            <div class="cv-item">
              <div class="cv-header">
                UX Consultant / AEIOU Foundation
              </div>
              <div class="cv-footer">
                Jun 2019 | Brisbane, Australia
              </div>
              <ul>
                <li>
                  Evaluated the current website by conducting contextual inquiry with the receptionists who have close contact with target users
                </li>
                <li>
                  Redesigned the information architecture based on the UX research
                </li>
              </ul>
            </div>
          </div>

          <div class="side-grey-line">
            <div>That’s pretty much about myself. Have a look of <a href="/">MY WORK</a> and let me know what you think!</div>
            <br>
            <div>Feel free to grab my resume <a href="/">HERE</a>.</div>
          </div>
        </div>
      </div>
    </div>
    <Footer />
  </div>
</template>

<style scoped>
.grey {
  background-color: #F5F5F5;
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

.padding-right { grid-area: padding-right; }

.padding-left { grid-area: padding-left; }

</style>

<script>
import Footer from '~/components/Footer.vue'
import TopBar from '~/components/TopBar.vue'
export default {
  components: {
    TopBar,
    Footer
  }
}
</script>
