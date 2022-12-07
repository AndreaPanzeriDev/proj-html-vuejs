<template>
  <div id="maps">
    <div class="mapouter">
      <div class="gmap_canvas">
        <iframe
          width="1000"
          height="500"
          id="gmap_canvas"
          src="https://maps.google.com/maps?q=trafalgar%20square&t=&z=13&ie=UTF8&iwloc=&output=embed"
          frameborder="0"
          scrolling="no"
          marginheight="0"
          marginwidth="0"
        ></iframe
        ><a href="https://123movies-to.org"></a><br /><a
          href="https://www.embedgooglemap.net"
          >how to embed google map in wordpress</a
        >
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
#maps {
  margin-top: 50px;
}

iframe {
  width: 100vw;
  height: 100%;
}

.mapouter {
  position: relative;
  text-align: right;
  height: 500px;
  width: 100vw;
}

.gmap_canvas {
  overflow: hidden;
  background: none !important;
  height: 500px;
  width: 100vw;
}
</style>