<template>
  <div id="sponsor" class="bsand py-25">
    <div class="container text-center ">
      <h1>SPONSORS</h1>
      <div>
        Maecenas faucibus mollis interdum. Nullam id dolor id nibh ultricies
        vehicula ut id elit.
      </div>
      <div class="d-flex space-between mt-50">
        <div v-for="(ele, index) in arraySponsor.length" :key="index">
            <img :src="require(`../assets/img/${arraySponsor[index]}`)" alt="banner sponsor">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "sponsorComp",
  props: {
    arraySponsor: Array,
  },
};
</script>

<style scoped>
.container{
    width: 70%;
    margin: auto;
}
</style>