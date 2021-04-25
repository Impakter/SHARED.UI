<template>
<div>
  <b-card id="cardItemLarge">
    <b-card-header id="headerIcon"><b-icon :icon="cardIcon"></b-icon></b-card-header>
    
    <b-card-title>{{cardTitle}}</b-card-title>
    <b-card-sub-title>{{cardSubtitle}}</b-card-sub-title>

    <slot></slot>

    <b-button id="btnArrow" @click="btnAction"><b-icon icon="arrow-right"></b-icon></b-button>
  </b-card>
</div>
</template>

<script> 
export default {
  name: 'CardItemLarge',
  props: {
    cardTitle: String,
    cardIcon: String
  }
}

</script>

<style scoped>

#cardItemLarge{
text-align: left;
max-width: 40rem;
box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
border: none;
}
#headerIcon{
padding: 0;
text-align: left;
font-size: 60px;
background-color: transparent;
border: none;
}
#btnArrow{
    float: right;
    background: transparent;
    color: #1D2029;
    width: 250px;
    border: none;
    font-size: 30px;
    font-weight: bold;
    text-align: right;
  }
</style>