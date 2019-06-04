<template>
  <div>
    <Layout :show-logo="false" style="z-index:99; position: relative">
      <!-- Author intro -->
      <Author :show-title="true"/>
      <!-- List posts -->
      <div class="posts">
        <PostCard v-for="edge in $page.posts.edges" :key="edge.node.id" :post="edge.node"/>
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
{
  posts: allPost {
    edges {
      node {
        id
        title
        path
        tags {
          id
          title
          path
        }
        date (format: "D. MMMM YYYY")
        timeToRead
        description
        coverImage (width: 770, height: 380, blur: 10)
        ...on Post {
            id
            title
            path
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
    title: "Hello, world!"
  }
};
</script>
