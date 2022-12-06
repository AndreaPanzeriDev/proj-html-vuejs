<template>
  <div id="News" class="d-flex space-between">
    <Card v-for="(elem, index) in arrayRecentNews" :key="index" :singleItem="elem" class="split d-flex"/>
  </div>
</template>

<script>

import Card from './card/recentNewsCard.vue'

export default {
    name: 'recentNews',
    components:{
        Card
    },
    props:{
      arrayRecentNews: Array
    }
}
</script>

<style scoped>
#News{
    width: 70%;
    margin: auto;
    display: flex;
    margin-top: 25px;
    color: #c6c1bd;
    height: 200px;  
}
.split{
    width: calc(100% / 3 - 15px);
}
</style>