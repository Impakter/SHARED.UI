<template>
  <div id="app">
<news-article :articleImage="'ArticleImage'" :articleTitle="'ArticleTitle'">Content of the article</news-article>
  </div>
</template>

<script>
import NewsArticle from './components/NewsArticle.vue'

export default {
  name: 'App',
  components: {
    NewsArticle
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
