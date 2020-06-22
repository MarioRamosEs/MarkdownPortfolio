<template>
  <Layout :show-logo="false">
    <Author :show-title="true" />
    <Categories />
  </Layout>
</template>

<script>
import Author from "~/components/Author.vue";
import Categories from "~/components/Categories.vue";

export default {
  components: {
    Author,
    Categories,
  },
  metaInfo: {
    title: "Inicio",
  },
};
</script>
