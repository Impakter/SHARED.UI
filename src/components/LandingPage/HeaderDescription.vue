<template>
<div id="hdDescription">
<h1 id="hdTitle">{{headerTitle}}</h1>
<h4 id="hdSubtitle">{{headerSubtitle}}</h4>
<slot></slot>
</div>    
</template>

<script>
export default {
  name: 'HeaderDescription',
  props: {
    headerTitle: String,
    headerSubtitle: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#hdDescription{
  font-family: 'Montserrat';
  padding: 10px;
  text-align: left;
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
