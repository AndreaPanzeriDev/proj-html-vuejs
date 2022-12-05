<template>
  <div id="speakerComp">
    <div class="contaier">
      <span>SPEAKERS</span>
      <div class="d-flex container_profession">
        <i class="fa-solid fa-angles-left"></i>
        <div v-for="(el, index) in 4" :key="index">
          <img :src="require(`../../assets/img/${arraySpeakers[position + index].person}`)" alt="profile picture">
        </div>
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
      position : 3
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