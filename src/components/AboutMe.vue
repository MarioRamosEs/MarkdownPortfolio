<template>
  <div>
    <div class="post-card content-box">
      <div class="post-card__content">
        <h2 class="post-card__title">About Me</h2>
        <p>
          FullStack Developer focused in .NET Core, Azure and Generative AI.
          Although I also like to program video games and other things in my
          spare time. Eager to learn more every day. 👨‍💻
        </p>
        <p>
          Most of the projects I have worked for are private, but here I show
          some of the ones that are public. (check the tabs above! ⬆️)
        </p>
        <p>
          <v-icon>mdi-email</v-icon>
          <a
            href="mailto:marioramosmontesinos@gmail.com"
            style="padding-left: 6px"
            >marioramosmontesinos@gmail.com</a
          >
        </p>
      </div>
    </div>

    <div class="post-card content-box">
      <div class="post-card__content">
        <h2 class="post-card__title">Tech Stack</h2>
        <p v-if="false" class="post-card__description">HOLA</p>
        <img src="/images/stack.png" alt="Tech Stack" />
      </div>
    </div>

    <div class="post-card content-box">
      <div class="post-card__content">
        <h2 class="post-card__title">Work experience</h2>
        <v-timeline dense>

<v-timeline-item>
            <template #icon>
              <v-avatar>
                <img src="/images/encamina_logo.jpeg" />
              </v-avatar>
            </template>
            <v-card class="elevation-2">
              <v-card-title class="headline">ENCAMINA - AI Cloud Solutions Dev</v-card-title>
              <v-card-subtitle
                >(jun. 2023 - nowadays)
                <v-chip-group>
                  <dot-net-chip></dot-net-chip>
                  <azure-chip></azure-chip>
                  <open-ai-chip></open-ai-chip>
                  <semantic-kernel-chip></semantic-kernel-chip>
                  <langchain-chip></langchain-chip>
                </v-chip-group>
              </v-card-subtitle>
              <v-card-text class="pl-0 pr-0">
                <ul>
                  <li>
                    Research and development of solutions using Azure OpenAI and GPT. Involved in projects such as questions and answers about documents, real-time summarization, 
                    execution of actions in a semantic way, among others.
                  </li>
                  <li>
                    Development of chatbots with Azure Bot Service and Azure Cognitive Services.
                  </li>
                  <li>
                    Full-stack development of custom applications for large companies.
                  </li>
                </ul>
              </v-card-text>
            </v-card>
          </v-timeline-item>

          <v-timeline-item>
            <template #icon>
              <v-avatar>
                <img src="/images/axpe_logo.png" />
              </v-avatar>
            </template>
            <v-card class="elevation-2">
              <v-card-title class="headline">AXPE Consulting - Fullstack Dev</v-card-title>
              <v-card-subtitle
                >(feb. 2021 - jun. 2023)
                <v-chip-group>
                  <dot-net-chip></dot-net-chip>
                  <angular-chip></angular-chip>
                  <azure-chip></azure-chip>
                  <jasper-reports-chip></jasper-reports-chip>
                </v-chip-group>
              </v-card-subtitle>
              <v-card-text class="pl-0 pr-0">
                <ul>
                  <li>
                    Development of the Hipatia platform, a restart from scratch
                    of the VHIR (Vall d'Hebron Research Institute) management
                    platform adaptable to other clinical research centers.
                  </li>
                  <li>
                    Decision making and quality manager on the technical part
                  </li>
                </ul>
              </v-card-text>
            </v-card>
          </v-timeline-item>
          <v-timeline-item>
            <template #icon>
              <v-avatar>
                <img src="/images/AtInfoserveis_logo.jpg" />
              </v-avatar>
            </template>
            <v-card class="elevation-2">
              <v-card-title class="headline">AT Infoserveis - Fullstack Dev</v-card-title>
              <v-card-subtitle
                >(sept. 2018 - dec. 2020)
                <v-chip-group>
                  <dot-net-chip></dot-net-chip>
                  <vue-chip></vue-chip>
                  <react-native-chip></react-native-chip>
                </v-chip-group>
              </v-card-subtitle>
              <v-card-text class="pl-0 pr-0">
                <ul>
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
            <template #icon>
              <v-avatar>
                <img src="/images/SLS_logo.jpg" />
              </v-avatar>
            </template>
            <v-card class="elevation-2">
              <v-card-title class="headline"
                >Serendipity Learning Services - STEM Educational coordinator</v-card-title
              >
              <v-card-subtitle>(sept. 2015 - jun. 2018)
                <v-chip-group>
                  <unity-chip></unity-chip>
                  <arduino-chip></arduino-chip>
                  <processing-chip></processing-chip>
                </v-chip-group>
              </v-card-subtitle>
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
        <h2 class="post-card__title">Certifications</h2>
        <v-timeline dense>
          <v-timeline-item>
            <template #icon>
              <v-avatar>
                <img src="/images/microsoft-certified-associate-badge.svg" />
              </v-avatar>
            </template>
            <v-card class="elevation-2">
              <v-card-title class="headline"
                >Microsoft Certified: Azure AI Engineer Associate</v-card-title
              >
              <v-card-subtitle
                >Microsoft - 2024 -
                <a
                  href="https://learn.microsoft.com/es-es/users/marioramos-7745/credentials/certification/azure-ai-engineer"
                  target="_blank"
                  >View credential</a
                ></v-card-subtitle
              >
            </v-card>
          </v-timeline-item>
          <v-timeline-item>
            <template #icon>
              <v-avatar>
                <img src="/images/azure-developer-associate-600x600.png" />
              </v-avatar>
            </template>
            <v-card class="elevation-2">
              <v-card-title class="headline"
                >Microsoft Certified: Azure Developer Associate</v-card-title
              >
              <v-card-subtitle
                >Microsoft - 2022 -
                <a
                  href="https://learn.microsoft.com/es-es/users/marioramos-7745/credentials/certification/azure-developer"
                  target="_blank"
                  >View credential</a
                ></v-card-subtitle
              >
            </v-card>
          </v-timeline-item>
          <v-timeline-item>
            <template #icon>
              <v-avatar>
                <img src="/images/azure-fundamentals-300x300.png" />
              </v-avatar>
            </template>
            <v-card class="elevation-2">
              <v-card-title class="headline"
                >Microsoft Certified: Azure Fundamentals</v-card-title
              >
              <v-card-subtitle
                >Microsoft - 2021 -
                <a
                  href="https://www.credly.com/badges/a554b5ce-0044-42dd-b171-59e8703b05c5/public_url"
                  target="_blank"
                  >View credential</a
                ></v-card-subtitle
              >
            </v-card>
          </v-timeline-item>
          <v-timeline-item>
            <template #icon>
              <v-avatar>
                <img src="/images/udemy.jfif" />
              </v-avatar>
            </template>
            <v-card class="elevation-2">
              <v-card-title class="headline"
                >Vuejs 2 + Vuex with TypeScript
              </v-card-title>
              <v-card-subtitle
                >Udemy - 2019 -
                <a
                  href="http://ude.my/UC-aba96422-c2f5-4e67-9a2c-570212e7e499"
                  target="_blank"
                  >View credential</a
                ></v-card-subtitle
              >
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
            <template #icon>
              <v-avatar>
                <img src="/images/UOC2.jpeg" />
              </v-avatar>
            </template>
            <v-card class="elevation-2">
              <v-card-title class="headline"
                >Computer Engineering Degree</v-card-title
              >
              <v-card-subtitle
                >Universitat Oberta de Catalunya UOC (2018 -
                nowadays)</v-card-subtitle
              >
            </v-card>
          </v-timeline-item>
          <v-timeline-item>
            <template #icon>
              <v-avatar>
                <img src="/images/EscolaPia_Logo.png" />
              </v-avatar>
            </template>
            <v-card class="elevation-2">
              <v-card-title class="headline"
                >Certificate of Higher Education in Multiplatform App
                Development</v-card-title
              >
              <v-card-subtitle
                >Escola Pia Santana (2016 - 2018)</v-card-subtitle
              >
            </v-card>
          </v-timeline-item>
          <v-timeline-item>
            <template #icon>
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
            <template #icon>
              <v-avatar>
                <img src="/images/marf_logo.png" />
              </v-avatar>
            </template>
            <v-card class="elevation-2">
              <v-card-title class="headline">S.T.E.M. Academy</v-card-title>
              <v-card-subtitle>MARF Informática (2010 - 2015)</v-card-subtitle>
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
                <template #default="{}">
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
                  <template #default="{}">
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
                  <template #default="{}">
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
<!--                <li>
                  <a href="https://spacetaco.studio/">Space Taco Studio</a>
                </li>
                <p>Game developer Studio</p>-->
                <li>
                  <a
                    href="https://www.amazon.es/Programaci%C3%B3n-Visual-Scratch-Marco-Rodr%C3%ADguez/dp/846176899X/ref=sr_1_1?__mk_es_ES=%C3%85M%C3%85%C5%BD%C3%95%C3%91&dchild=1&keywords=programacion+visual+con+scratch&qid=1608118096&sr=8-1"
                    >Programación visual con Scratch</a
                  >
                </li>
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
import AzureChip from "./TechChips/AzureChip";
import DotNetChip from "./TechChips/DotNetChip";
import AngularChip from "./TechChips/AngularChip";
import VueChip from "./TechChips/VueChip";
import ReactNativeChip from "./TechChips/ReactNativeChip";
import JasperReportsChip from "./TechChips/JasperReportsChip";
import UnityChip from "./TechChips/UnityChip";
import ArduinoChip from "./TechChips/ArduinoChip";
import ProcessingChip from "./TechChips/ProcessingChip";
import OpenAiChip from "./TechChips/OpenAiChip";
import LangchainChip from "./TechChips/LangchainChip";
import SemanticKernelChip from "./TechChips/SemanticKernelChip";

export default {
  components: {
    ProcessingChip,
    ArduinoChip,
    UnityChip,
    JasperReportsChip,
    ReactNativeChip,
    VueChip,
    AngularChip,
    DotNetChip,
    AzureChip,
    OpenAiChip,
    LangchainChip,
    SemanticKernelChip,
  },
};
</script>

<style lang="scss">
h5 {
  margin-top: 0px;
}

.theme--light.v-sheet--outlined {
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
