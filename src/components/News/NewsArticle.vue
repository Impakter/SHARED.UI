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

.article{
  height: 200px;
  width: 300px;
  border: 2px solid rgb(161, 161, 161);
  border-radius: 20px;
}

</style>
