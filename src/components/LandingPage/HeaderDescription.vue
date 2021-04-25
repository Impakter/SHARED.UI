<template>
<div id="hdDescription">
<h1 id="hdTitle">{{headerTitle}}</h1>
<h4 id="hdSubtitle">{{headerSubtitle}}</h4>
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
#hdDescription{
  height: 200px;
  padding: 5px;
  text-align: left;
  width: 300px;
  border: none;
}
#hdTitle{
    text-transform: uppercase;
    font-weight:bold;
}
#hdSubtitle{
    font-weight:bold;
}

</style>
