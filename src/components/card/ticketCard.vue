<template>
  <div>
    <div class="w-100">
      <div class="bsand py-15">
        <h2 class="text-center  fw-bold o-7">{{singleItem.name}}</h2>
        <div class="text-center scarlet fw-bold ">{{singleItem.price}}</div>
        <div class="bwhite py-15">
          <div v-for="(elem, n) in singleItem.bonus.length" :key="n">
          <div class="text-center my-15">{{singleItem.bonus[n]}}</div>
          </div>
        </div>
      </div>
      <div class="bscarlet py-15">
        <div class="text-white text-center fw-bold fs-1">BOOK NOW</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ticketCard',
  props:{
    singleItem: Object,
  },
  mounted(){
  }
}
</script>

<style scoped>

</style>