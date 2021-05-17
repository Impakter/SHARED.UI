<template>
<a class="newsLink" :href="newsLink" target="_blank">
 <b-card class="article" :img-src="articleImage" img-alt="Card image" img-top>
    <b-card-title> {{articleTitle}} </b-card-title>
        <b-card-text>
          <slot></slot>
    </b-card-text>
 </b-card>
 </a>
</template>

<script>
export default {
  name: 'NewsArticle',
  props: {
    articleTitle: String,
    articleImage: String,
    newsLink: String,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
*{
  font-family: 'Montserrat', sans-serif;
}
.article{
  border: none;
  border-radius: 3px;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
  max-width: 20rem;
  text-align: left;
  overflow: hidden;
}
.card-title{
  font-weight: 700;
  
}
.card-text{
  font-size: 14px;
}
.img{
  max-height: 15rem;
}
/* a{
  text-decoration: none!important;
  text-decoration-color: none!important;;
} */

.newsLink, a:link, a:visited {
  color: black;
    text-decoration: none;
}

</style>
