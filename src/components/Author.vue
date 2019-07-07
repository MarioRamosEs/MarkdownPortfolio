<template>
  <div class="author">
    <g-image alt="Author image" class="author__image" src="~/assets/images/author2.jpg" />

    <h1 v-if="showTitle" class="author__site-title">{{ $static.metaData.siteName }}</h1>

    <p class="author__intro">FullStack Developer</p>

    <p class="author__links">
      <a href="https://github.com/MarioRamosEs">GitHub</a>
      <a href="http://marioramos.es/DATA/CV_MarioRamos_2018.pdf">CV</a>
    </p>
  </div>
</template>

<static-query>
query {
  metaData {
    siteName
  }
}
</static-query>

<script>
export default {
  props: ["showTitle"]
};
</script>

<style lang="scss">
.author {
  margin: 0 auto;
  max-width: 500px;
  text-align: center;
  padding: calc(var(--space) / 2) 0;

  &__image {
    border-radius: 100%;
    width: 150px;
    height: 150px;
    margin-bottom: 1em;
  }

  &__intro {
    opacity: 0.8;
  }

  &__site-title {
    font-size: 1.5em;
  }

  &__links {
    margin-top: -0.5em;
    a {
      margin: 0 0.5em;
    }
  }
}
</style>