<template>
  <div id="questionComp">
    <QuestionCard v-for="(elem, index) in arrayAboutUs" :key="index" :singleItem="elem" class="split d-flex"/>
  </div>
</template>

<script>

import QuestionCard from './card/QuestionCard.vue'

export default {
  components:{
    QuestionCard
  },
  props:{
    arrayAboutUs: Array
  }
}
</script>

<style scoped>
#questionComp{
    width: 70%;
    margin: auto;
    display: flex;
    margin-top: 25px;
    color: #c6c1bd;
    
}
.split{
    width: calc(100% / 3);
}

</style>