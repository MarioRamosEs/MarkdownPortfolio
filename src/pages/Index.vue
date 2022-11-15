<template>
  <Layout :show-logo="false">
    <!-- Author intro -->
    <Author :show-title="true" />

    <br>
    <br>
    <div class="posts">
      <v-tabs centered icons-and-text show-arrows>
        <v-tab>About me<v-icon>mdi-account</v-icon></v-tab>
        <v-tab>Azure<v-icon>mdi-microsoft-azure</v-icon></v-tab>
        <v-tab>Web<v-icon>mdi-web</v-icon></v-tab>
        <v-tab>Apps<v-icon>mdi-cellphone-arrow-down</v-icon></v-tab>
        <v-tab>I+D / IA<v-icon>mdi-clipboard-search-outline</v-icon></v-tab>
        <v-tab>Games<v-icon>mdi-gamepad-square</v-icon></v-tab>
        <v-tab-item class="pt-2">
          <AboutMe />
        </v-tab-item>
        <v-tab-item class="pt-2">
          <PostCard
            v-for="edge in $page.azure.edges"
            :key="edge.node.id"
            :post="edge.node"
          />
        </v-tab-item>
        <v-tab-item class="pt-2">
          <PostCard
            v-for="edge in $page.web.edges"
            :key="edge.node.id"
            :post="edge.node"
          />
        </v-tab-item>
        <v-tab-item class="pt-2">
          <PostCard
            v-for="edge in $page.app.edges"
            :key="edge.node.id"
            :post="edge.node"
          />
        </v-tab-item>
        <v-tab-item class="pt-2">
          <PostCard
            v-for="edge in $page.others.edges"
            :key="edge.node.id"
            :post="edge.node"
          />
        </v-tab-item>
        <v-tab-item class="pt-2">
          <PostCard
            v-for="edge in $page.games.edges"
            :key="edge.node.id"
            :post="edge.node"
          />
        </v-tab-item>
      </v-tabs>
    </div>
  </Layout>
</template>

<page-query>
query {
  azure: allPost(filter: { published: { eq: true }, tags: { contains: "Azure" }}) {
    edges {
      node {
        id
        title
        date (format: "D. MMMM YYYY")
        timeToRead
        description
        cover_image (width: 770, height: 380, blur: 10)
        path
        tags {
        id
        title
        path
        }
      }
    }
  },
  web: allPost(filter: { published: { eq: true }, tags: { contains: "Web" }}) {
    edges {
      node {
        id
        title
        date (format: "D. MMMM YYYY")
        timeToRead
        description
        cover_image (width: 770, height: 380, blur: 10)
        path
        tags {
          id
          title
          path
        }
      }
    }
  },
  app: allPost(filter: { published: { eq: true }, tags: { contains: "App" }}) {
    edges {
      node {
        id
        title
        date (format: "D. MMMM YYYY")
        timeToRead
        description
        cover_image (width: 770, height: 380, blur: 10)
        path
        tags {
          id
          title
          path
        }
      }
    }
  },
  games: allPost(filter: { published: { eq: true }, tags: { contains: "Game" }}) {
    edges {
      node {
        id
        title
        date (format: "D. MMMM YYYY")
        timeToRead
        description
        cover_image (width: 770, height: 380, blur: 10)
        path
        tags {
          id
          title
          path
        }
      }
    }
  },
  others: allPost(filter: { published: { eq: true }, tags: { contains: "I+D" }}) {
    edges {
      node {
        id
        title
        date (format: "D. MMMM YYYY")
        timeToRead
        description
        cover_image (width: 770, height: 380, blur: 10)
        path
        tags {
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
import Categories from "~/components/Categories.vue";
import PostCard from "~/components/PostCard.vue";
import AboutMe from "~/components/AboutMe.vue";

export default {
  components: {
    Author,
    PostCard,
    Categories,
    AboutMe,
  },
  metaInfo: {
    title: "Portfolio",
  },
};
</script>
