<template>
  <div id="speakerComp">
    <div class="contaier">
      <div class="space-between d-flex align-items-center">
        <span class="fs-2">SPEAKERS</span>
        <div>
          <button class="button ms-5 text-white" @click="goBack">&lt;</button>
          <button class="button ms-5 text-white" @click="goOn">></button>
        </div>
      </div>
      <div class="d-flex space-around mt-50">
        <div v-for="(el, index) in 4" :key="index">
          <div class="container2">
            <img
              :src="
                require(`../../assets/img/${
                  arraySpeakers[position + index].person
                }`)
              "
              alt="profile picture"
            />
            <div class="img_overlay">
              <i class="fa-brands fa-twitter fs-1 ms-5"></i>
              <i class="fa-brands fa-square-facebook fs-1 ms-5"></i>
              <i class="fa-brands fa-linkedin-in fs-1 ms-5"></i>
            </div>
          </div>

          <h3 class="text-center">
            {{ arraySpeakers[position + index].name }}
          </h3>
          <div class="text-center dustyGray italic">
            {{ arraySpeakers[position + index].job }}
          </div>
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
  methods: {
    goOn() {
      console.log(this.position);
      if (this.position == 4) {
        this.position = 0;
      } else {
        this.position++;
      }
    },

    goBack() {
      console.log(this.position);
      if (this.position == 0) {
        this.position = 4;
      } else {
        this.position--;
      }
    },
  },
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

img {
  width: 222px;
  border-radius: 20px;
}
.container2:hover{
  position: relative;
  display: flex;
  justify-content: center;
  align-content: center;
}

.img_overlay{
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0;
  left: 0;
  margin-right: -50%;
  color: white;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #f7260c;
  opacity: 0.6;
  border-radius: 20px;
}
</style>