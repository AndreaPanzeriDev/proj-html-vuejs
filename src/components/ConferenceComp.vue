<template>
  <div id="conference">
    <div>CONFERENCE ON</div>
    <div>SOCIAL NETWORKS</div>
    <div>**************************</div>
    <div>IEONCIOECN / ORNFOIRN / OENROEINR</div>
    <div>bottone</div>
  </div>
</template>

<script>
export default {
    name: "ConferenceComp",
    data(){
        return{
            slider:[
                {background: '../assets/img/slider-1-bg.jpg', position:'center'},
                {background: '../assets/img/2-item-1.jpg', position: 'right'},
                {},
            ],
            position: 0,
        }  
    },
    methods(){

    }
}
</script>

<style scoped>
#conference{
    background-image: url('../assets/img/slider-1-bg.jpg');
    width: 100%;
    height: 100%;
    color: white;
}
</style>