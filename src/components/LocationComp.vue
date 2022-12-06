<template>
  <div id="location">
    <div class="m-auto">
        <div class="text-white fw-bold fs-3 text-center">LOCATION</div>
        <div class="text-white fw-bold fs-2">GB BUILDING, GRAND CONFERENCE ROOM</div>
        <div class="d-flex text-white justify-content-center">
            <div><i class="fa-solid fa-location-arrow"></i></div>
            <div class="ms-5">11 GD Building, River Mall, New York, USA 8879</div>
        </div>
        <div class="text-center my-30">
            <a class="italic" href="#">Click for accomodation here</a>
        </div>
        <div class="text-center">
            <img src="../assets/img/1-item-2.jpg" alt="bar">
        </div>
        <div class="d-flex justify-content-center mt-20">
            <div class="d-flex text-white">
                <i class="fa-solid fa-phone mr-10"></i>
                <div>+1-112-222-3344</div>
            </div>
            <div class="d-flex text-white">
                <i class="fa-solid fa-envelope mr-30"></i>
                <div>contactme@mrpriest.gmail.com</div>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'LocationComp'
}
</script>

<style scoped>
#location{
    background-image: url('../assets/img/location-bg.jpg');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    width: 100%;
    display: flex;
    height: 500px;
}

a{
    color: #f7260c;
}

</style>