<template>
  <body>
    <div class="title">
      <h1 class="title-h1">Aurore Langelier</h1>
      <h2 class="title-h2">Software Engineer</h2>

      <title-icons />
    </div>
    <div class="container">
      <div class="timeline-item" date-is="January 2023 - August 2025">
        <h1>
          <b-link href="https://www.leboncoin.fr/" target="_blank"
            ><img src="~/static/lbc.png" height="30rem"
          /></b-link>
          Backend Engineer @Leboncoin
        </h1>
        <div class="wrapper-columns">
          <div class="left-column div1">
            <p>
              Backend engineer in charge of the secure transaction lifecycle for
              the vehicle marketplace.
            </p>
            <p>
                Architected and implemented the secured payment feature
                <ul>
                  <li>From classified ad eligibility to user-to-user checkout</li>
                  <li>Sending notifications based on the ad lifecycle</li>
                </ul>
            </p>
            <p>
              Help architect and implement legacy distributed monolith into
              Go-based microservices.
            </p>
            <p>
              Contributed to platform-level backend guild and cross-team
              reliability improvements.
            </p>
          </div>
          <div class="right-column div2">
            <p></p>
            <p><br />SCRUM, GitHub, Gerrit</p>
            <p><br />Golang, PgSQL, Cron, DDD</p>
            <p><br />Concourse, Datadog, Grafana</p>
          </div>
        </div>
      </div>

      <div class="timeline-item" date-is="January 2019 - January 2023">
        <h1>
          <img src="~/static/peevee.png" height="30rem" />
          Software Engineer @Peevee
        </h1>
        <div class="wrapper-columns">
          <div class="left-column div1">
            <p>
              Joint-venture
              <b-link href="https://www.verteego.com" target="_blank"
                >Verteego</b-link
              >
              x
              <b-link href="https://www.experis.com" target="_blank"
                >Experis</b-link
              >
            </p>
            <p>Human-size team : 4 devs, 1 data scientist, 1 PO.</p>
            <p>
              Powee : a product focused on improving IT support for Manpower
              agents through a chat bot answering questions, searching through
              knowledge bases and handling tickets.
            </p>
            <p>
              Backoffice product focused on managing knowledge bases and
              configuring Powee instances.
            </p>
            <p>
              Helped our data scientist industrialize machine learning models
              for production.
            </p>
            <p>
              In charge of regular releases, bug fixes and crisis management.
            </p>
          </div>
          <div class="right-column div2">
            <p></p>
            <p><br />SCRUM, Git</p>
            <p><br />NodeJS, Express, Postgresl, Dialogflow, GCP</p>
            <p><br />Vue.js, HTML/CSS, GCP</p>
            <p><br />Python, Flask, GCP</p>
          </div>
        </div>
      </div>

      <div class="timeline-item" date-is="May 2018 - September 2018">
        <h1>
          <img src="~/static/matlo.png" height="30rem" /> Front end developer
          intern @Matlo
        </h1>
        <div class="wrapper-columns">
          <div class="left-column div1">
            <p>Front end developer in a 10 people startup.</p>
            <p>
              Maintenance and evolution of Matlo, a data visualization platform.
            </p>
            <p>
              Bug fixes, design and development of new features and design of
              exploratory dashboards
            </p>
          </div>
          <div class="right-column div2">
            <p></p>
            <p><br />Javascript ES6, Typescript, React, Vega</p>
          </div>
        </div>
      </div>

      <div class="timeline-item" date-is="June 2017 - August 2017">
        <h1>
          <b-link href="https://www.hibox.co/" target="_blank"
            ><img src="~/static/hibox.png" height="30rem"
          /></b-link>
          Full stack developer intern @Hibox
        </h1>
        <div class="wrapper-columns">
          <div class="left-column div1">
            <p>Full stack developer in a 12 people startup.</p>
            <p>
              Design and development of two web apps: SASS tool for creating
              data visualizations and "changelog as a service".
            </p>
            <p>
              Released on
              <a href="https://www.getbeamer.com/" target="_blank"
                >getbeamer.com</a
              >
            </p>
          </div>
          <div class="right-column div2">
            <p></p>
            <p><br />Java, Hibernate, Struts2, Javascript, Chart.js</p>
          </div>
        </div>
      </div>

      <div class="timeline-item" date-is="2013 - 2018">
        <h1>
          <b-link href="https://polytech.univ-nantes.fr/" target="_blank"
            ><img src="~/static/polytech.png" height="30rem"
          /></b-link>
          Bs and Ms @Polytech Nantes
        </h1>
        <div class="wrapper-columns">
          <div class="left-column div1">
            <p>
              BS of Math & Physics. Ms of Computer Science specialized in
              Business Intelligence.
            </p>
            <p>
              Disrupt’ Campus, double degree in innovation and design thinking.
            </p>
            <p>Engineering School of Polytech Nantes (Nantes, France).</p>
          </div>
        </div>
      </div>
    </div>
  </body>
</template>

<script>
import titleIcons from "~/components/titleIcons.vue";

export default {
  name: "IndexPage",
  components: {
    titleIcons,
  },
};
</script>
<style scoped>
@import url("https://fonts.googleapis.com/css?family=Oswald|Roboto:400,700");

.wrapper-columns {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}

.left-column {
  display: flex;
  flex-direction: column;
  width: 50%;
  padding: 1em;
}

.right-column {
  display: flex;
  flex-direction: column;
  width: 50%;
  border-left: 2px solid rgba(0, 0, 0, 0.3);
  padding: 1em;
}

.div2 {
  opacity: 0;
}

.div1:hover ~ .div2 {
  opacity: 1;
}

body {
  font-size: 14px;
  line-height: 1.5;
}

h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: "Oswald", sans-serif;
}

h1 {
  font-size: 2rem;
  margin-bottom: 0.5em;
}

p {
  font-family: "Roboto", sans-serif;
  font-size: 0.8rem;
}

.title {
  max-width: 1024px;
  width: 50%;
  margin: 0 auto;
}

.title-h1 {
  font-size: 3rem;
  text-align: center;
}

.title-h2 {
  text-align: center;
  color: rgba(0, 0, 0, 0.7);
}

.title-icons {
  font-size: 1.5em;
  text-align: center;
  color: rgba(0, 0, 0, 0.7);
}

.container {
  max-width: 1024px;
  width: 90%;
  margin: 0 auto;
}

.timeline-item {
  padding: 3em 2em 2em;
  position: relative;
  color: rgba(0, 0, 0, 0.7);
  border-left: 2px solid rgba(0, 0, 0, 0.3);
}

.timeline-item p {
  font-size: 1rem;
}

.timeline-item::before {
  content: attr(date-is);
  position: absolute;
  left: 2em;
  font-weight: bold;
  top: 1em;
  display: block;
  font-family: "Roboto", sans-serif;
  font-weight: 700;
  font-size: 0.785rem;
}

.timeline-item::after {
  width: 10px;
  height: 10px;
  display: block;
  top: 1em;
  position: absolute;
  left: -7px;
  border-radius: 10px;
  content: "";
  border: 2px solid rgba(0, 0, 0, 0.3);
  background: white;
}

.timeline-item:last-child {
  border-image: linear-gradient(
      to bottom,
      rgba(0, 0, 0, 0.3) 60%,
      rgba(0, 0, 0, 0)
    )
    1 100%;
}
</style>
