<template>
  <div id="app">
    <HeaderComp/>
    <MainComp :arrayAboutUs="aboutUs" :arraySpeakers="speakers"/>
  </div>
</template>

<script>
import HeaderComp from './components/HeaderComp.vue'
import MainComp from './components/MainComp.vue'

export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp,
  },
  data(){
    return{
      aboutUs: [
        {icon: 'fa-solid fa-trophy', title: 'WHO WE ARE', phrase:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Veniam perspiciatis, dolorum distinctio id facere nam maiores'},
        {icon: 'fa-solid fa-bolt', title: 'WHAT WE DO', phrase:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Veniam perspiciatis, dolorum distinctio id facere nam maiores'},
        {icon: 'fa-solid fa-question', title: 'WHY US', phrase:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Veniam perspiciatis, dolorum distinctio id facere nam maiores'},
      ],
      speakers: [
        {person: 'speaker-1-150x150.jpg', name: 'PATRICK SPENCER', job: 'S&P Analyzer'},
        {person: 'speaker-2-150x150.jpg', name: 'JANET JONES', job: "NewYork Post't GM"},
        {person: 'speaker-3-150x150.jpg', name: 'MICHEAL DOVER', job: "Starbuck's CEO"},
        {person: 'speaker-4-150x150.jpg', name: 'ANGELINA HOLY', job: "Maxii's Manager"},
        {person: 'speaker-5-150x150.jpg', name: 'PATRICK SPENCER', job: 'S&P Analyzer'},
        {person: 'speaker-6-150x150.jpg', name: 'PATRICK SPENCER', job: 'S&P Analyzer'},
        {person: 'speaker-7-150x150.jpg', name: 'PATRICK SPENCER', job: 'S&P Analyzer'},
        {person: 'speaker-8-150x150.jpg', name: 'PATRICK SPENCER', job: 'S&P Analyzer'},
      ],
    }
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}



.d-flex {
  display: flex;
}

.text-center{
  text-align: center;
}

.justify-content-center{
  justify-content: center;
}

.text-white{
  color: white;
}

.fw-bold{
  font-weight: bold;
}

.ms-5{
  margin: 0 5px;
}

.mt-50{
  margin-top: 50px;
}

.fs-2{
  font-size: 2rem;
}

.align-self-center{
  align-self: center;
}

.text-black{
  color: black;
}

.button{
  padding: 10px 15px;
  border: none;
  border-radius: 5px;
  background-color: #f7260c;
}

.m-auto{
  margin: auto;
}

.space-around{
  justify-content: space-around;
}
</style>
