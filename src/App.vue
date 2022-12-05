<template>
  <div id="app">
    <HeaderComp/>
    <MainComp/>
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

html{
  padding: 0;
  margin: 0;
  box-sizing: 0;
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

.button{
  padding: 10px 15px;
  border: none;
  border-radius: 5px;
  background-color: #f7260c;
}
</style>
