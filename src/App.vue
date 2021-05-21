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
           <b-row>
             <news-article 
             :articleImage="'https://placekitten.com/600/400'" 
             :articleTitle="'title of the article'" 
             :newsLink="'https://impakter.com/ashden-meet-the-pioneers-boosting-rights-and-resilience-in-earths-threatened-forests/'">
             The last week in April was marked by the announcement of new, more ambitious climate
              goals from two of the world’s largest polluters, the United States and Europe. 
             Could they be a turning point in the fight against climate change?</news-article>
             <social-media-article 
             :articleImage="'https://placekitten.com/600/400'" 
             :smIcon="'twitter'"
             :articleTitle="'title of the article'" 
             :newsLink="'https://impakter.com/ashden-meet-the-pioneers-boosting-rights-and-resilience-in-earths-threatened-forests/'">
             The last week in April was marked by the announcement of new, more ambitious climate
              goals from two of the world’s largest polluters, the United States and Europe. 
             Could they be a turning point in the fight against climate change?</social-media-article>
                
           </b-row>
        </b-container>  
        </b-tab>
        <b-tab title="Landing Page">
         <b-container>
          <header-description 
            :headerTitle="'Header Title'" 
            :headerSubtitle="' Header Subtitle'">
            Description Goes Here: Sed sed felis posuere, tempor ipsum at, lacinia tortor. 
            Mauris mattis, mauris non pretium sodales, lacus arcu lacinia nunc, ut aliquam
            lacus lectus id purus. Aliquam erat volutpat.
          </header-description>
          <action-button 
            :btnIcon ="'person'" 
            :btnDescription="'Description of Button'"
            :btnAction="src='/home'" 
          />
          <card-item 
            :cardTitle="'Card Title'" 
            :cardIcon="'folder2-open'" 
            :iconColor="'purple'" 
            :buttonIcon="'arrow-right'" 
            :btnLink="'/home'">
            Description goes Here: Sed sed felis posuere, tempor ipsum at, 
            lacinia tortor, mauris mattis,
             mauris non pretium sodales
          </card-item>
         <card-item-large 
            :cardTitle="'Card Title'" 
            :cardIcon="'folder2-open'" 
            :iconColor="'red'">
            Description goes Here: Sed sed felis posuere, tempor ipsum at, 
            lacinia tortor, Mauris mattis, mauris non pretium sodales
         </card-item-large>
          </b-container>
        </b-tab>
        <b-tab title="User Components">
          <profile-picture :profilePic="'https://placekitten.com/300/400'"></profile-picture>
        </b-tab>
        <b-tab title="Industries">
          <b-card-text>content</b-card-text>
        </b-tab>
        
      </b-tabs>
      
    </b-card >
    <hr />


  </div>
</template>

<script>
import NewsArticle from './components/News/NewsArticle.vue'
import SocialMediaArticle from './components/News/SocialMediaArticle'
import HeaderDescription from './components/LandingPage/HeaderDescription'
import ActionButton from './components/LandingPage/ActionButton'
import CardItem from './components/LandingPage/CardItem'
import CardItemLarge from './components/LandingPage/CardItemLage'
import ProfilePicture from './components/User/ProfilePicture'


export default {
  name: 'App',
  components: {
    NewsArticle,
    HeaderDescription,
    ActionButton,
    CardItem,
    CardItemLarge,
    SocialMediaArticle,
    ProfilePicture,
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
