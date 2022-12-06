<template>
  <div id="presentation" class="d-flex">
    <div class="w-50">
      <div class="fs-2 o-7 mt-50">PRESENTATION</div>
      <div>
        <video-embed
          src="https://www.youtube.com/watch?v=pfDuIBjzIIo"
          class="mt-20"
        ></video-embed>
        <div></div>
      </div>
    </div>
    <div class="w-50">
      <div class="fs-2 o-7 mt-50">TWITTER FEED</div>

      <div v-for="(elem, index) in arrayTwitter.length" :key="index">
        <div class="d-flex my-20">
          <div class="lightblue ms-5"><i class="fa-brands fa-twitter"></i></div>
          <div>{{ arrayTwitter[index] }}</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "presentationComp",
  props: {
    arrayTwitter: Array,
  },
};
</script>

<style scoped>
#presentation {
  width: 70%;
  margin: auto;
}

img {
  max-width: 90%;
  position: relative;
}
</style>