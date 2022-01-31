<template>
  <div>
    <div class="post-card content-box">
      <div class="post-card__content">
        <h2 class="post-card__title">About Me</h2>
        <p>
          FullStack Developer focused in .NET Core, Azure and Angular/Vue. 
          Although I also like to program video games and other things in
          my spare time. Eager to learn more every day. 👨‍💻
        </p>
        <p>
          Most of the projects I have worked for are private, but here I show
          some of the ones that are public.
        </p>
      </div>
    </div>

    <div class="post-card content-box">
      <div class="post-card__content">
        <h2 class="post-card__title">Tech Stacks</h2>
        <p class="post-card__description" v-if="false">HOLA</p>
        <img src="/images/stacks.png" alt="Tech Stacks" />
      </div>
    </div>

    <div class="post-card content-box">
      <div class="post-card__content">
        <h2 class="post-card__title">Work experience</h2>
        <v-timeline dense>
                    <v-timeline-item>
            <template v-slot:icon>
              <v-avatar>
                <img src="/images/axpe_logo.png" />
              </v-avatar>
            </template>
            <v-card class="elevation-2">
              <v-card-title class="headline">AXPE Consulting</v-card-title>
              <v-card-subtitle>(feb. 2021 - nowadays)</v-card-subtitle>
              <v-card-text class="pl-0 pr-0">
                <ul>
                  <li>
                    Net Core, Angular
                  </li>
                  <li>
                    Development of the Hipatia platform, a restart from scratch of the VHIR (Vall d'Hebron Research Institute) management platform adaptable to other clinical research centers.
                  </li>
                </ul>
              </v-card-text>
            </v-card>
          </v-timeline-item>
          <v-timeline-item>
            <template v-slot:icon>
              <v-avatar>
                <img src="/images/AtInfoserveis_logo.jpg" />
              </v-avatar>
            </template>
            <v-card class="elevation-2">
              <v-card-title class="headline">AT Infoserveis</v-card-title>
              <v-card-subtitle>(sept. 2018 - dec. 2020)</v-card-subtitle>
              <v-card-text class="pl-0 pr-0">
                <ul>
                  <li>
                    Vue.js, React Native and .NET
                  </li>
                  <li>
                    Development of customized platforms. Websites and
                    cross-platform apps.
                  </li>
                  <li>
                    Development of integrations with A3ERP. Synchronizers,
                    websites, apps and plant management software.
                  </li>
                  <li>
                    Development of integrations with Prestashop, Salesforce,
                    Zoho, WooComerce and Consentio.
                  </li>
                  <li>Online and face-to-face assistance for any problem.</li>
                </ul>
              </v-card-text>
            </v-card>
          </v-timeline-item>
          <v-timeline-item>
            <template v-slot:icon>
              <v-avatar>
                <img src="/images/SLS_logo.jpg" />
              </v-avatar>
            </template>
            <v-card class="elevation-2">
              <v-card-title class="headline"
                >Serendipity Learning Services</v-card-title
              >
              <v-card-subtitle>(sept. 2015 - jun. 2018)</v-card-subtitle>
              <v-card-text>
                <ul>
                  <li>
                    Collaborating in the creation of STEM projects related to
                    web, robotics, IoT and video games.
                  </li>
                </ul>
              </v-card-text>
            </v-card>
          </v-timeline-item>
        </v-timeline>
      </div>
    </div>

    <div class="post-card content-box">
      <div class="post-card__content">
        <h2 class="post-card__title">Studies</h2>
        <v-timeline dense>
          <v-timeline-item>
            <template v-slot:icon>
              <v-avatar>
                <img src="/images/UOC2.jpeg" />
              </v-avatar>
            </template>
            <v-card class="elevation-2">
              <v-card-title class="headline"
                >Computer Engineering Degree</v-card-title
              >
              <v-card-subtitle>Universitat Oberta de Catalunya UOC (2018 - nowadays)</v-card-subtitle>
            </v-card>
          </v-timeline-item>
          <v-timeline-item>
            <template v-slot:icon>
              <v-avatar>
                <img src="/images/EscolaPia_Logo.png" />
              </v-avatar>
            </template>
            <v-card class="elevation-2">
              <v-card-title class="headline"
                >Certificate of Higher Education in Multiplatform App
                Development</v-card-title
              >
              <v-card-subtitle>Escola Pia Santana (2016 - 2018)</v-card-subtitle>
            </v-card>
          </v-timeline-item>
          <v-timeline-item>
            <template v-slot:icon>
              <v-avatar>
                <img src="/images/biada_logo.jpg" />
              </v-avatar>
            </template>
            <v-card class="elevation-2">
              <v-card-title class="headline"
                >Technological Baccalaureate</v-card-title
              >
              <v-card-subtitle>IES Miquel Biada (2014 - 2016)</v-card-subtitle>
            </v-card>
          </v-timeline-item>
          <v-timeline-item>
            <template v-slot:icon>
              <v-avatar>
                <img src="/images/marf_logo.png" />
              </v-avatar>
            </template>
            <v-card class="elevation-2">
              <v-card-title class="headline"
                >S.T.E.M. Academy</v-card-title
              >
              <v-card-subtitle>MARF Informática (2010 - 2015)</v-card-subtitle>
            </v-card>
          </v-timeline-item>
        </v-timeline>
      </div>
    </div>

     <div class="post-card content-box">
      <div class="post-card__content">
        <h2 class="post-card__title">Certifications</h2>
        <v-timeline dense>
          <v-timeline-item>
            <template v-slot:icon>
              <v-avatar>
                <img src="/images/azure-fundamentals-300x300.png" />
              </v-avatar>
            </template>
            <v-card class="elevation-2">
              <v-card-title class="headline"
                >Microsoft Certified: Azure Fundamentals</v-card-title
              >
              <v-card-subtitle>Microsoft - 2021 - <a href="https://www.youracclaim.com/badges/804c8832-c999-4952-94a8-804e019eeef9" target="_blank">View credential</a></v-card-subtitle>
            </v-card>
          </v-timeline-item>
          <v-timeline-item>
            <template v-slot:icon>
              <v-avatar>
                <img src="/images/udemy.jfif" />
              </v-avatar>
            </template>
            <v-card class="elevation-2">
              <v-card-title class="headline"
                >Vuejs 2 + Vuex with TypeScript </v-card-title
              >
              <v-card-subtitle>Udemy - 2019 - <a href="http://ude.my/UC-aba96422-c2f5-4e67-9a2c-570212e7e499" target="_blank">View credential</a></v-card-subtitle>
            </v-card>
          </v-timeline-item>
        </v-timeline>
      </div>
    </div>

    <div class="post-card content-box">
      <div class="post-card__content">
        <h2 class="post-card__title">More Info</h2>
        <v-row no-gutters>
          <v-col cols="12" sm="12" md="6">
            <v-card class="pa-2" outlined tile>
              <h5>Languages</h5>
              <v-progress-linear
                color="light-blue"
                height="25"
                value="100"
                striped
              >
                <template v-slot:default="{}">
                  <strong>Spanish</strong>
                </template></v-progress-linear
              >
              <div class="pt-2">
                <v-progress-linear
                color="light-blue"
                height="25"
                value="70"
                striped
              >
                <template v-slot:default="{}">
                  <strong>Catalan</strong>
                </template></v-progress-linear
              >
              </div>
              <div class="pt-2">
                <v-progress-linear
                color="light-blue"
                height="25"
                value="50"
                striped
              >
                <template v-slot:default="{}">
                  <strong>English</strong>
                </template></v-progress-linear
              >
              </div>
            </v-card>
          </v-col>
          <v-col cols="12" sm="12" md="6">
            <v-card class="pa-2" outlined tile> 
              <h5>Collaborations</h5>
              <ul>
                <li><a href="https://spacetaco.studio/">Space Taco Studio</a></li>
                <p>Game developer Studio</p>
                <li><a href="https://www.amazon.es/Programaci%C3%B3n-Visual-Scratch-Marco-Rodr%C3%ADguez/dp/846176899X/ref=sr_1_1?__mk_es_ES=%C3%85M%C3%85%C5%BD%C3%95%C3%91&dchild=1&keywords=programacion+visual+con+scratch&qid=1608118096&sr=8-1">Programación visual con Scratch</a></li>
                <p>Formative Book</p>
              </ul>
               </v-card>
          </v-col>
        </v-row>
      </div>
    </div>
  </div>
</template>
ˆ
<script>
export default {};
</script>

<style lang="scss">

h5{
  margin-top: 0px;
}

.theme--light.v-sheet--outlined{
  border: none;
}

.post-card {
  margin-bottom: var(--space);
  position: relative;
  max-width: 800px;
  box-shadow: 1px 10px 30px 0 rgba(0, 0, 0, 0.2);

  &:hover {
    transform: translateY(-5px);
    box-shadow: 1px 10px 30px 0 rgba(0, 0, 0, 0.3);
  }

  &__header {
    margin-left: calc(var(--space) * -1);
    margin-right: calc(var(--space) * -1);
    margin-bottom: calc(var(--space) / 2);
    margin-top: calc(var(--space) * -1);
    overflow: hidden;
    border-radius: var(--radius) var(--radius) 0 0;

    &:empty {
      display: none;
    }
  }

  &__image {
    min-width: 100%;
  }

  &__title {
    margin-top: 0;
  }

  &__tags {
    z-index: 1;
    position: relative;
  }

  &__link {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    opacity: 0;
    overflow: hidden;
    text-indent: -9999px;
    z-index: 0;
  }
}
</style>
