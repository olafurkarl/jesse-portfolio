<template>
  <div>
    <div class="container">
      <div class="content grey">
        <div class="padding-left" />
        <div class="padding-right" />
        <TopBar />
      </div>
      <div class="content about">
        <div class="padding-left" />
        <div class="padding-right" />
        <div class="center">
          <div class="about-intro">
            <img src="~assets/about/jesse-sunglasses.png">

            <div class="greeting-text">
              I’m <span class="name">Jesse Ting</span>, a Product Designer based in Sydney Australia
            </div>
          </div>
          <div class="about-me">
            <div class="side-grey-line">
              <h3>About Me</h3>
              <div class="text">
                Hi there! My real name is 丁建宇 which pronouces as Ding Jian-Yu, but Jesse will do.
                I was born and raised in Taipei, Taiwan with a passion for human-centred design, and I embrace challenges,
                problem solving processes, and team collaboration. I love going for a walk when pondering complex problems or a run to reboot my design engine.
                I hope to bring humanity into technology which empowers us to do greater work.
              </div>
            </div>
          </div>

          <div class="side-by-side">
            <div class="side-grey-line">
              <h3>Education</h3>
              <ul class="list-stretch">
                <li>
                  <div class="cv-header">
                    Queensland University of Technology
                  </div>
                  <div class="cv-text">
                    Master of IT - User Experience track
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

            <div class="side-grey-line specialties">
              <h3>Specialties</h3>
              <ul class="list-stretch">
                <li>
                  UX Research
                </li>
                <li>Product Design</li>
                <li>Interaction Design</li>
                <li>Prototyping </li>
                <li>Usability Testing</li>
                <li>Problem Solving</li>
                <li>Wireframing</li>
                <li>Business Process Management</li>
                <li>Heuristic Review</li>
              </ul>
            </div>
          </div>

          <div class="experience">
            <div class="side-grey-line">
              <h3>Experience</h3>
              <div class="cv-item">
                <div class="cv-header">
                  Product Designer / Vai
                </div>
                <div class="cv-footer">
                  Sep 2020 - Present | Sydney, Australia
                </div>
                <ul>
                  <li>
                    Informing product design decisions by providing contextual user research.
                  </li>
                  <li>
                    Collaborating with the development team to build the design system on Figma.
                  </li>
                  <li>
                    Delivering Hi-fi prototypes and specified design handovers to the development team.
                  </li>
                  <li>
                    Using techniques such as Card Sorting, A/B Testing, Heuristic Review, Usability Testing to optimise the products’ UX.
                  </li>
                </ul>
              </div>
              <div class="cv-item">
                <div class="cv-header">
                  UX Designer / Quokka Technology
                </div>
                <div class="cv-footer">
                  Jun 2020 - December 2020 | Remote
                </div>
                <ul>
                  <li>
                    Evaluated the web product by using Heuristic Review.
                  </li>
                  <li>
                    Conducted User Interviews to understand pain points and to validate the hypotheses and assumptions.
                  </li>
                  <li>
                    Collaborated with other designers on my team to solve complex problems.
                  </li>
                </ul>
              </div>
              <div class="cv-item">
                <div class="cv-header">
                  UX/UI Designer / Conversions King
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
          </div>

          <div class="about-outro">
            <div class="side-grey-line">
              <div>
                That’s pretty much about myself. Have a look of <nuxt-link v-smooth-scroll :to="{ path: '/', hash:'#projects'}" href="/#projects" class="topbar-about nostyle">
                  MY WORK
                </nuxt-link> and let me know what you think!
              </div>
              <br>
              <div>Feel free to grab my resume <a href="/resume.pdf" download="Jesse Ting (Jian-Yu) Resume.pdf" class="topbar-about nostyle">HERE</a>.</div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <Footer />
  </div>
</template>

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

<style scoped>
a {
  text-decoration: underline;
  color: #E35975;
}

.nuxt-link-exact-active, .nuxt-link-active {
  text-decoration: underline;
  color: #E35975;
}

.grey {
  background-color: #F5F5F5;
}

.cv-item {
  margin-top: 2em;
}

.cv-item li {
  font-family: Lato;
  font-style: normal;
  font-weight: 300;
  font-size: 20px;
  margin-bottom: 5px;
}

.cv-header {
  font-family: Lato;
  font-style: normal;
  font-weight: 500;
  font-size: 20px;
  color: #003C72;
}

.cv-text {
  font-family: Lato;
  font-style: normal;
  font-weight: 300;
  font-size: 24px;
}

.cv-footer {
  font-family: Lato;
  font-style: normal;
  font-weight: normal;
  font-size: 18px;
  color: #929292;
}

.about-outro {
  margin-top: 3em;
  font-family: Montserrat;
  font-style: normal;
  font-weight: 500;
  font-size: 30px;
  line-height: 37px;
  display: flex;
  margin-bottom: 3em;
}

@media(max-width: 420px) {
  .about-outro {
    font-size: 18px;
  }
}

.about-outro > div {
  padding: 1em;
}

.about-me, .experience {
  width: 100%;
  margin-top: 3em;
}

@media (max-width: 420px) {
  .experience {
    margin-top: 6em;
  }
}

.about-intro img {
  max-width: 500px;
  width: 100%;
  object-fit: cover;
}

.side-by-side {
  margin-top: 3em;
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: 1fr;
  grid-column-gap: 5%;
}

@media (max-width: 420px) {
  .side-by-side {
    margin-top: 3em;
    display: grid;
    grid-template-columns: 1fr;
    grid-template-rows: auto auto;
    grid-row-gap: 5%;
    grid-column-gap: 0;
  }
}

.side-grey-line {
  border-left: 2px solid #AAAAAA;
  padding-left: 2em;
}

.text {
  margin-top: 1em;
  line-height: 35px;
  font-size: 20px;
}

@media(max-width: 420px) {
  .text {
    font-size: 14px;
    line-height: 24px;
  }
}

.about-intro {
  display: grid;
  grid-template-columns: fit-content(500px) 1fr;
  grid-template-rows: 1fr;

  align-items: center;
  grid-column-gap: 5%;

  margin-top: 4em;
}

@media (max-width: 420px) {
  .about-intro {
    display: grid;
    grid-template-columns: 1fr;
    grid-template-rows: fit-content(500px) 1fr;
    align-items: center;
    grid-row-gap: 5%;
    margin-top: 4em;
    text-align: center;
  }
}

.greeting-text {
  font-family: Montserrat;
  font-style: normal;
  font-weight: 600;
  font-size: 4vw;
}

.name {
  color: #E35975;
}

.list-stretch {
  display: grid;
  align-items: center;
  height: 90%;
  padding-top: 5%;
  list-style-position: inside;
  list-style-type: none;
  padding-left: 0;
  align-content: space-between;
  grid-row-gap: 10px;
}

.list-stretch li {
  align-self: end;
}

.experience ul {
  list-style-type: none;
  padding-left: 1em;
}

.experience ul li::before {
  content: "\25E6";
  color: #003C72;;
  display: inline-block;
  width: 0.5em;
  margin-left: -0.5em;
}

.experience .cv-footer {
  line-height: 35px;
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

.about {
  font-family: Lato;
  font-weight: 300;
}

.about h3 {
  font-family: Montserrat;
  font-style: normal;
  font-weight: normal;
  font-size: 24px;
  line-height: 29px;
}

.specialties li {
  font-family: Lato;
  font-style: normal;
  font-weight: normal;
  font-size: 22px;
  line-height: 35px;
  letter-spacing: 0.06em;
  font-weight: 300;
}

@media(max-width: 420px) {
  .specialties li {
    font-size: 14px;
  }

  .list-stretch {
    grid-row-gap: 10px;
  }

  .cv-header, .cv-text, .cv-item li {
    font-size: 14px;
  }

  .cv-footer {
    font-size: 12px;
  }

  .side-grey-line {
    padding-left: 1em;
  }
}

</style>
