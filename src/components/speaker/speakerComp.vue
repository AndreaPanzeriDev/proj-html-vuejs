<template>
  <div id="speakerComp">
    <div class="contaier">
      <div class="space-between d-flex align-items-center">
        <span class="fs-2">SPEAKERS</span>
        <div>
          <button class="button ms-5" @click="goBack">x</button>
          <button class="button ms-5" @click="goOn">></button>
        </div>
      </div>
      <div class="d-flex space-around mt-50">
        <div v-for="(el, index) in 4" :key="index">
          <img
            :src="
              require(`../../assets/img/${
                arraySpeakers[position + index].person
              }`)
            "
            alt="profile picture"
          />
          <h3 class="text-center">{{arraySpeakers[position + index].name}}</h3>
          <div class="text-center dustyGray italic">{{arraySpeakers[position + index].job}}</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "speakerComp",
  props: {
    arraySpeakers: Array,
  },
  data() {
    return {
      position: 0,
    };
  },
  methods:{
    goOn(){
      console.log(this.position)
      if(this.position == 4){
        this.position = 0;
      }else{
        this.position++;
      }
    },

    goBack(){
      console.log(this.position)
      if(this.position == 0){
        this.position = 4;
      }else{
        this.position--;
      }
    }
  }
};
</script>

<style scoped>
#speakerComp {
  background-color: #f3f3f3;
}

.contaier {
  width: 70%;
  margin: auto;
  padding: 50px 0;
}

.contaier > span {
  font-size: 30px;
}


</style>