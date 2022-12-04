<template>
  <div id="conference"></div>
</template>

<script>
export default {
  name: "ConferenceComp",
  data(){
    return{
        slider:[
            {
                img: '../assets/img/slider-1-bg.jpg',
                phrases: {
                    e: { p: 'CONFERENCE ON', font: 25, color: '#f0776b' },
                    e: { p: 'SOCIAL NETRWORKS', font: 25, color: '#f0776b' },
                    e: { p: '-----------------------------------', font: 25, color: '#f0776b' },
                    e: { p: '23 -26 MAY 2019  /  SAN FRANCISCO /  8 SPEAKERS', font: 25, color: '#f0776b' },
                },
                display_location: 'center'
            },
            {
                img: '../assets/img/slider-1-bg.jpg', //da cambiare
                phrases: {
                    e: { p: 'MEET', font: 25, color: '#f0776b' },
                    e: { p: 'SOME EXPERTS', font: 15, color: '#ffffff' },
                },
                display_location: 'right'
            },
        ],
    }
  }
};
</script>

<style scoped>

</style>