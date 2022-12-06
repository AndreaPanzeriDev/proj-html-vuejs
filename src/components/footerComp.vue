<template>
  <div id="footer">
    <div class="bblack o-7">
      <div class="container d-flex py-25 space-between">
        <div class="w-20">
          <div class="text-white">ABOUT US</div>
          <div class="text-white py-15">
            Cum sociis natoque penatibus et magnis dis parturient montes,
            nascetur ridiculus mus.
          </div>
          <div class="d-flex space-around">
            <a href="#"
              ><i class="fa-brands fa-square-facebook text-white fs-1"></i
            ></a>
            <a href="#"
              ><i class="fa-brands fa-square-twitter text-white fs-1"></i
            ></a>
            <a href="#"
              ><i class="fa-brands fa-linkedin text-white fs-1"></i
            ></a>
            <a href="#"
              ><i class="fa-brands fa-square-google-plus text-white fs-1"></i
            ></a>
            <a href="#"
              ><i class="fa-brands fa-square-pinterest text-white fs-1"></i
            ></a>
          </div>
        </div>
        <div class="w-20">
          <div class="text-white">RECENT NEWS</div>
          <div class="flex pt-15">
            <i class="fa-solid fa-caret-right text-white"></i>
            <a href="#" class="text-white">Sem Porta Mollis Parturient</a>
          </div>
          <div class="flex">
            <i class="fa-solid fa-caret-right text-white"></i>
            <a href="#" class="text-white">Nullam Lorem Mattis Purus</a>
          </div>
          <div class="flex">
            <i class="fa-solid fa-caret-right text-white"></i>
            <a href="#" class="text-white">Nibh Sem Sit Ullamcorper</a>
          </div>
          <div class="flex">
            <i class="fa-solid fa-caret-right text-white"></i>
            <a href="#" class="text-white">Donec luctus imperdiet</a>
          </div>
          <div class="flex">
            <i class="fa-solid fa-caret-right text-white"></i>
            <a href="#" class="text-white">Magna pars studiorum</a>
          </div>
        </div>
        <div class="w-20">
          <div class="text-white">GET YOUR SEAT!</div>
          <p class="text-white">
            Book for your seat before it's too rate. We provide variety of
            ticket options.
          </p>
          <a href="#"
            ><button class="button text-white">CHECK OUT TICKETS!</button></a
          >
        </div>
        <div class="w-20">
          <div class="text-white">GALLERY FROM THE LAST YEAR</div>
          <div>
            <div class="d-flex space-between wrap">
              <card
                v-for="(elem, index) in arrayGallery"
                :key="index"
                :singleItem="elem"
              />
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="bblack o-9 py-25">
      <div class="container d-flex space-between">
        <div class="text-white">© Copyright GoodLayers, All Right Reserved</div>
        <div class="d-flex">
            <div><a class="text-white mr-10" href="#">About us |</a></div>
            <div><a class="text-white mr-10" href="#">Accomadation |</a></div>
            <div><a class="text-white mr-10" href="#">Call for Paper |</a></div>
            <div><a class="text-white" href="#">Contact Us</a></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import card from "./card/footerCard.vue";

export default {
  name: "footerComp",
  components: {
    card,
  },
  props: {
    arrayGallery: Array,
  },
};
</script>

<style scoped>
.container {
  width: 70%;
  margin: auto;
}

.wrap {
  flex-wrap: wrap;
}

.slice {
  width: calc(100% / 4 - 5px);
  flex-wrap: wrap;
}
</style>