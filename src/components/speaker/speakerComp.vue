<template>
  <div id="speakerComp">
    <div class="contaier">
        <span class="fw-bold">SPEAKERS</span>
        <div class="d-flex container_profession">
          <i class="fa-solid fa-angles-left"></i>
            <div v-for="(elem, index) in arraySpeakers" :key="index" :singleItem="elem"></div>
          <i class="fa-solid fa-angles-right"></i>
        </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "speakerComp",
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