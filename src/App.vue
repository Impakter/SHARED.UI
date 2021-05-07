<template>

  <div id="app">  
    <b-card no-body>
      <b-tabs card>
        <b-tab title="Basic UI" active>
          <b-card-text>
          </b-card-text>
        </b-tab>
        <b-tab title="News Components">
         <b-container>
           <news-article :articleImage="'https://placekitten.com/380/200'" :articleTitle="'title of the article'">The last week in April was marked by the announcement of new, more ambitious climate goals from two of the world’s largest polluters, the United States and Europe. Could they be a turning point in the fight against climate change?</news-article>
         </b-container>
          
        </b-tab>
        <b-tab title="Landing Page">
         <b-container>
          <header-description :headerTitle="'Header Title'" :headerSubtitle="' Header Subtitle'">Description Goes Here: Sed sed felis posuere, tempor ipsum at, lacinia tortor.  Mauris mattis, mauris non pretium sodales, lacus arcu lacinia nunc, ut aliquam lacus lectus id purus. Aliquam erat volutpat.</header-description>
          <action-button :btnIcon ="'person'" :btnDescription="'Description of Button'"/>
          <card-item :cardTitle="'Card Title'" :cardIcon="'folder2-open'" :iconColor="'purple'" :buttonIcon="'arrow-right'">Description goes Here: Sed sed felis posuere, tempor ipsum at, lacinia tortor, mauris mattis, mauris non pretium sodales</card-item>
         <card-item-large :cardTitle="'Card Title'" :cardIcon="'folder2-open'" :iconColor="'red'">Description goes Here: Sed sed felis posuere, tempor ipsum at, lacinia tortor, Mauris mattis, mauris non pretium sodales</card-item-large>
          </b-container>
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
import HeaderDescription from './components/LandingPage/HeaderDescription'
import ActionButton from './components/LandingPage/ActionButton'
import CardItem from './components/LandingPage/CardItem'
import CardItemLarge from './components/LandingPage/CardItemLage'


export default {
  name: 'App',
  components: {
    NewsArticle,
    HeaderDescription,
    ActionButton,
    CardItem,
    CardItemLarge,
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
