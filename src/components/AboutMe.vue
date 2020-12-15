<template>
  <div>
    <div class="post-card content-box">
      <div class="post-card__content">
        <h2 class="post-card__title">About Me</h2>
        <p>
          Young FullStack Developer focused in .NET Core, Vue, React Native and
          Azure. Although I also like to program video games and other things in
          my spare time. Eager to learn more every day. 👨‍💻
        </p>
        <p>
          Most of the projects I have worked for are private, but here I show
          some of the ones that are public. Currently looking for a job in
          Barcelona 😉
        </p>
      </div>
    </div>

    <div class="post-card content-box">
      <div class="post-card__content">
        <h2 class="post-card__title">Tech Stacks</h2>
        <p class="post-card__description" v-if="false">HOLA</p>
        <img src="/images/Stacks.png" alt="Tech Stacks" />
      </div>
    </div>

    <div class="post-card content-box">
      <div class="post-card__content">
        <h2 class="post-card__title">Work experience</h2>
        <v-timeline dense>
          <v-timeline-item>
            <template v-slot:icon>
              <v-avatar>
                <img src="/images/AtInfoserveis_logo.jpg" />
              </v-avatar>
            </template>
            <v-card class="elevation-2">
              <v-card-title class="headline">AT Infoserveis</v-card-title>
              <v-card-subtitle>(sept. 2018 - nov. 2020)</v-card-subtitle>
              <v-card-text>
                <ul>
                  <li>
                    Development of customized platforms. Websites and cross-platform apps.
                  </li>
                  <li>
                    Development of integrations with A3ERP. Synchronizers, websites, apps and plant management software.
                  </li>
                  <li>
                    Development of integrations with Prestashop, Salesforce, Zoho, WooComerce and Consentio.
                  </li>
                  <li>
                    Online and face-to-face assistance for any problem.
                  </li>
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
              <v-card-title class="headline">Serendipity Learning Services</v-card-title>
              <v-card-subtitle>(sept. 2015 - jun. 2018)</v-card-subtitle>
              <v-card-text>
                <ul>
                  <li>Collaborating in the creation of STEM projects related to web, robotics, IoT and video games.</li>
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
              <v-card-title class="headline">Computer Engineering Degree - UOC</v-card-title>
              <v-card-subtitle>(2018 - nowadays)</v-card-subtitle>
            </v-card>
          </v-timeline-item>
          <v-timeline-item>
            <template v-slot:icon>
              <v-avatar>
                <img src="/images/EscolaPia_Logo.png" />
              </v-avatar>
            </template>
            <v-card class="elevation-2">
              <v-card-title class="headline">Certificate of Higher Education in Multiplatform App Development</v-card-title>
              <v-card-subtitle>(2016 - 2018)</v-card-subtitle>
            </v-card>
          </v-timeline-item>
        </v-timeline>
      </div>
    </div>

  </div>
</template>
ˆ
<script>
export default {};
</script>

<style lang="scss">
.post-card {
  margin-bottom: var(--space);
  position: relative;
  max-width: 800px;
  box-shadow: 1px 10px 30px 0 rgba(0, 0, 0, 0.1);

  &:hover {
    transform: translateY(-5px);
    box-shadow: 1px 10px 30px 0 rgba(0, 0, 0, 0.1);
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
