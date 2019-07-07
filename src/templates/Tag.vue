<template>
  <div>
    <Layout style="z-index:99; position: relative">
      <h1 class="tag-title text-center space-bottom"># {{ $page.tag.title }}</h1>

      <div class="posts">
        <PostCard v-for="edge in $page.tag.belongsTo.edges" :key="edge.node.id" :post="edge.node"/>
      </div>
    </Layout>
    <vue-particles
      style="position: fixed;
        top: 0;
        width: 100%"
      color="#fff"
      class="container"
      moveSpeed="2"
    ></vue-particles>
  </div>
</template>

<page-query>
query Tag ($id: String!) {
  tag (id: $id) {
    title
    belongsTo {
      edges {
        node {
          ...on Post {
            title
            path
            date (format: "D. MMMM YYYY")
            timeToRead
            description
            coverImage (width: 860, blur: 10)
            content
          }
        }
      }
    }
  }
}
</page-query>

<script>
import Author from "~/components/Author.vue";
import PostCard from "~/components/PostCard.vue";

export default {
  components: {
    Author,
    PostCard
  },
  metaInfo: {
    title: "Etiquetas"
  }
};
</script>

<style lang="scss">
</style>

