<template>

  <div class="image">{{imageUrl}}</div>

</template>

<script>
export default {
  name: 'HeaderImage',
  props: {
    imageUrl: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.image{
  min-height: 250px;
  max-width: 800px;
  background: #BBBBBB;

}
</style>
