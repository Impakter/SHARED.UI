<template>
<div class="article">
<h3>{{articleTitle}}</h3>
<div>{{articleImage}}</div>
<slot></slot>
</div>    
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

</style>
