<template>
 <b-card class="article" :img-src="articleImage" img-alt="Card image" img-top>
    <b-card-title> {{articleTitle}} </b-card-title>
        <b-card-text>
          <slot></slot>
    </b-card-text>
 </b-card>
</template>

<script>
export default {
  name: 'NewsArticle',
  props: {
    articleTitle: String,
    articleImage: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.article{
  font-family: 'Montserrat';
  border: none;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
  max-width: 20rem;
}
</style>
