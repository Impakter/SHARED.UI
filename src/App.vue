<template>

  <div id="app">  
    <b-card no-body>
      <b-tabs card>
        <b-tab title="Basic UI" active>
          <b-card-text>
          </b-card-text>
        </b-tab>
        <b-tab title="News Components">
          <b-card-text>  
          </b-card-text>
          <news-article :articleImage="'image url'" :articleTitle="'title of the article'">Content of the article goes here</news-article>
        </b-tab>
        <b-tab title="Landing Page">
          <header-description :headerTitle="'Title'" :headerSubtitle="'Subtitle'">Description Goes Here</header-description>
          <header-image :imageUrl="'image url'"/>
          <action-button :btnIcon ="'person'" :btnDescription="'Description of Button'"/>
        </b-tab>
        <b-tab title="Industries">
          <b-card-text>content</b-card-text>
        </b-tab>
      </b-tabs>
    </b-card>
    <hr />


  </div>
</template>

<script>
import NewsArticle from './components/News/NewsArticle.vue'
import HeaderImage from './components/LandingPage/HeaderImage'
import HeaderDescription from './components/LandingPage/HeaderDescription'
import ActionButton from './components/LandingPage/ActionButton'

export default {
  name: 'App',
  components: {
    NewsArticle,
    HeaderImage,
    HeaderDescription,
    ActionButton
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
