<template>
  <div id="program" class="mt-50">
    <div class="container">
      <div class="d-flex space-around align-items-center">
        <span class="fs-2">PROGRAM</span>
        <div class="w-50">
          <span class="dustyGray"
            >This conference run through all 4 days from 23 -26 May 2016. We
            also provide free lunch and coffee break in each day
          </span>
        </div>
        <a class="italic scarlet" href="#">View Full Program</a>
      </div>
      <!--redone-->
      <div class="d-flex mt-20">
        <div class="w-20">
          <div class="fw-bold text-white">DAY 1</div>
          <div class="text-white">{{ arrayPrograms[0].date }}</div>
        </div>
        <div class="w-20">
          <div class="fw-bold text-white">DAY 2</div>
          <div class="text-white">{{ arrayPrograms[1].date }}</div>
        </div>
        <div class="w-20">
          <div class="fw-bold text-white">DAY 3</div>
          <div class="text-white">{{ arrayPrograms[2].date }}</div>
        </div>
        <div class="w-20">
          <div class="fw-bold text-white">DAY 4</div>
          <div class="text-white">{{ arrayPrograms[3].date }}</div>
        </div>
        <div class="w-20">
          <div class="fw-bold text-white">DAY 5</div>
          <div class="text-white">{{ arrayPrograms[4].date }}</div>
        </div>
      </div>
      <div class="bsand c_info d-flex pt-25">
        <div class="w-25">
          <div class="d-flex my-20 align-items-center text-center">
            <i class="fa-regular fa-clock dustyGray mr-10"></i>
            <div class="dustyGray">{{ arrayPrograms[position].time }}</div>
          </div>
          <div class="d-flex my-20 align-items-center text-center">
            <i class="fa-solid fa-location-arrow dustyGray mr-10"></i>
            <span class="dustyGray">ROOM A</span>
          </div>
          <div class="d-flex my-20 align-items-center text-center">
            <i class="fa-solid fa-user-large dustyGray mr-10"></i>
            <div class="dustyGray">{{ arrayPrograms[position].name }}</div>
          </div>
        </div>
        <div class="w-75">
          <div class="text-black o-7 fs-2 my-20">
            {{ arrayPrograms[position].title }}
          </div>
          <div class="text-black o-7">
            {{ arrayPrograms[position].description }}
          </div>
          <img
            :src="
              require(`../../assets/img/${arrayPrograms[position].picture}`)
            "
            alt="picture"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "programCard",
  props: {
    arrayPrograms: Array,
  },
  data() {
    return {
      position: 0,
    };
  },
};
</script>

<style scoped>
.container {
  width: 70%;
  margin: auto;
}

.w-20 {
  width: 20%;
  padding: 20px 10px;
  background-color: #f7260c;
}

.c_info {
  width: 100%;
  height: auto;
}
</style>