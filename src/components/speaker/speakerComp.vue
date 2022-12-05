<template>
  <div id="speakerComp">
    <div class="contaier">
        <span class="fw-bold">SPEAKERS</span>
        <speakerCard v-for="(elem, index) in arraySpeakers" :key="index" :singleItem="elem"/>
    </div>
  </div>
</template>

<script>

import speakerCard from './speakerCard.vue'

export default {
  name: "speakerComp",

  components:{
    speakerCard
  },
  props:{
    arraySpeakers: Array
  },
  data(){
    return{
      position : 0
    }
  }
};
</script>

<style scoped>
#speakerComp {
  background-color: #f3f3f3;
}

.contaier{
    width: 70%;
    margin: auto;
    padding: 50px 0;
}

.contaier > span {
    font-size: 30px;
}

.container_profession{
  justify-content: space-around;
}
</style>