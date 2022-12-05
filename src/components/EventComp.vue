<template>
  <div id="event">
    <div>
      <div class="text-center text-white conference_on animate delay-1">CONFERENCE ON</div>
      <div class="text-center text-white fw-bold social_networks animate delay-2">SOCIAL NETWORKS</div>
      <div class="text-center animate delay-3"><img src="../assets/img/1-item-2.jpg" alt="bar" /></div>
      <div class="d-flex justify-content-center text-white fw-bold">
        <div class="ms-5 animate delay-4">23 - 26 MAY 2019</div>
        <div class="ms-5 animate delay-5">/</div>
        <div class="ms-5 animate delay-6">SAN FRANCISCO</div>
        <div class="ms-5 animate delay-7">/</div>
        <div class="ms-5 animate delay-8">8 SPEAKERS</div>
      </div>
      <div class="text-center animate delay-9"><button class="button text-white mt-50">REGISTER ONLINE</button></div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
#event {
  width: 100%;
  height: 500px;
  background-image: url("../assets/img/slider-1-bg.jpg");
  background-repeat: no-repeat;
  background-position: center;
  display: flex;
  justify-content: center;
  align-items: center;
}

.conference_on{
  font-size: 48px;
}
.social_networks{
  font-size: 5rem;
}
/************************
       ANIMATION
************************/
.animate {
  animation-duration: 0.5s;
  animation-name: animate-fade;
  animation-delay: 0.5s;
  animation-fill-mode: backwards;
}
.animate.glow {
  animation-name: animate-glow;
  animation-timing-function: ease;
}

@keyframes animate-fade {
  0% { opacity: 0; }
  100% { opacity: 1; }
}

.delay-1 {
  animation-delay: 0.6s;
}
.delay-2 {
  animation-delay: 0.7s;
}
.delay-3 {
  animation-delay: 0.8s;
}
.delay-4 {
  animation-delay: 0.9s;
}
.delay-5 {
  animation-delay: 1s;
}
.delay-6 {
  animation-delay: 1.1s;
}
.delay-7 {
  animation-delay: 1.2s;
}
.delay-8 {
  animation-delay: 1.3s;
}
.delay-9 {
  animation-delay: 2s;
}
</style>