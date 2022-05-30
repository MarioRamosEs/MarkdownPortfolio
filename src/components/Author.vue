<template>
  <div class="author">
    <g-image
      alt="Author image"
      class="author__image"
      src="~/assets/images/author3.jpg"
      width="180"
      height="180"
    />

    <h1 v-if="showTitle" class="author__site-title">
      {{ $static.metadata.siteName }}
    </h1>

    <p class="author__intro">FullStack Developer in Barcelona</p>

    <v-row justify="center" align="center" style="padding: 10px">
      <v-btn
        outlined
        class="ma-2"
        color="primary"
        target="_blank"
        href="https://github.com/MarioRamosEs"
      >
        <v-icon left>
          mdi-github
        </v-icon>
        GitHub
      </v-btn>

      <v-btn
        outlined
        class="ma-2"
        color="primary"
        target="_blank"
        href="https://www.linkedin.com/in/marioramosmontesinos/"
      >
        <v-icon left>
          mdi-linkedin
        </v-icon>
        LinkedIn
      </v-btn>

      <v-btn
        outlined
        class="ma-2"
        color="primary"
        target="_blank"
        href="https://twitter.com/marioramoses"
      >
        <v-icon left>
          mdi-twitter
        </v-icon>
        Twitter
      </v-btn>

      <v-btn
        outlined
        class="ma-2"
        color="primary"
        target="_blank"
        href="CV_MarioRamos_2022.pdf"
      >
        <v-icon left>
          mdi-file-pdf-box
        </v-icon>
        CV 2022
      </v-btn>
    </v-row>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<script>
export default {
  props: ["showTitle"],
};
</script>

<style lang="scss">
.author {
  margin: 0 auto;
  max-width: 600px;
  text-align: center;
  padding: calc(var(--space) / 2) 0;
  padding-bottom: 0px;
  padding-top: 0px;

  &__image {
    border-radius: 100%;
    margin-bottom: 1em;
  }

  &__intro {
    opacity: 0.8;
  }

  &__site-title {
    font-size: 1.5em;
    margin-bottom: 0em;
  }

  &__links {
    margin-top: -0.5em;
    a {
      margin: 0 0.5em;
    }
  }
}

.glow-on-hover {
  margin: 5px;
  width: 100px;
  height: 50px;
  border: none;
  outline: none;
  color: #fff;
  background: #111;
  cursor: pointer;
  position: relative;
  z-index: 0;
  border-radius: 10px;
}

.glow-on-hover:before {
  content: "";
  background: linear-gradient(
    45deg,
    #ff0000,
    #ff7300,
    #fffb00,
    #48ff00,
    #00ffd5,
    #002bff,
    #7a00ff,
    #ff00c8,
    #ff0000
  );
  position: absolute;
  top: -2px;
  left: -2px;
  background-size: 400%;
  z-index: -1;
  filter: blur(5px);
  width: calc(100% + 4px);
  height: calc(100% + 4px);
  animation: glowing 20s linear infinite;
  opacity: 0;
  transition: opacity 0.3s ease-in-out;
  border-radius: 10px;
}

.glow-on-hover:active {
  color: #000;
}

.glow-on-hover:hover:before {
  opacity: 1;
}

.glow-on-hover:after {
  z-index: -1;
  content: "";
  position: absolute;
  width: 100%;
  height: 100%;
  background: #111;
  left: 0;
  top: 0;
  border-radius: 10px;
}

@keyframes glowing {
  0% {
    background-position: 0 0;
  }
  50% {
    background-position: 400% 0;
  }
  100% {
    background-position: 0 0;
  }
}
</style>
