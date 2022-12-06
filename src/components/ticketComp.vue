<template>
  <div id="ticket" class="mt-50">
    <div class="container">
      <div class="text-center text-white fs-3 fw-bold">TICKET</div>
      <div class="d-flex space-between">
        <Card v-for="(elem, index) in arrayTicket" :key="index" :singleItem="elem"   class="d-flex slice"/>
      </div>
    </div>
  </div>
</template>

<script>
import Card from "./card/ticketCard.vue";

export default {
  name: "ticketComp",
  components: {
    Card,
  },
  props: {
    arrayTicket: Array,
  },
};
</script>

<style scoped>
#ticket {
  height: 500px;
  background-image: url(../assets/img/ticket-bg.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}

.container{
  width: 70%;
  margin: auto;
}

.slice{
  width: calc(100% / 3 - 50px);
}
</style>