<template>
  <div id="subscribe">
    <div class="d-flex blocks">
      <div class="block">
        <h2>326</h2>
        <h6>giorni</h6>
      </div>
      <div class="block">
        <h2>326</h2>
        <h6>giorni</h6>
      </div>
      <div class="block">
        <h2>326</h2>
        <h6>giorni</h6>
      </div>
      <div class="block">
        <h2>326</h2>
        <h6>giorni</h6>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SubscribeComp",
};
</script>

<style scoped>
#subscribe {
  background-image: url("../assets/img/coutdown-bg1.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  width: 100%;
  margin-top: 50px;
  height: 500px;
  display: flex;
  justify-content: center;
}



.block {
  background-color: black;
  opacity: 0.7;
  padding: 2px 20px;
  border-radius: 5px;
  margin: auto 5px;
  color: white;
}
</style>