<template>
<div class="hdDescription">
<h1>{{headerTitle}}</h1>
<h5>{{headerSubtitle}}</h5>
<slot></slot>
</div>    
</template>

<script>
export default {
  name: 'NewsArticle',
  props: {
    headerTitle: String,
    headerSubtitle: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hdDescription{
  height: 200px;
  width: 300px;
  border: 2px solid #BBBBBB;
  border-radius: 5px;
}
</style>
