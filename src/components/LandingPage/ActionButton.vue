<template>
    
   <b-button id="accButton" @click="btnAction" ><b-icon :icon="btnIcon"></b-icon>{{ btnDescription }}</b-button>
</template>

<script>
export default {
  name: 'ActionButton',
  props: {
    btnDescription: String,
    btnIcon: String,
    btnAction: String
  }
}
</script>

<style scoped>
#accButton{
    display: inline-block;
    background: white;
    color: #1D2029;
    width: 250px;
    border-radius: 5px;
    border: 2px solid #989898;
    white-space: nowrap;
    font-weight: bold;
  }
</style>