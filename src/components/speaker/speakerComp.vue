<template>
  <div id="speakerComp">
    <div class="contaier">
      <div class="space-between d-flex align-items-center">
        <span class="fs-2">SPEAKERS</span>
        <div>
          <button class="button ms-5">x</button>
          <button class="button ms-5">></button>
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
      position: 3,
    };
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

</style>