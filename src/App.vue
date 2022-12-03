<template>
  <div id="app">
    <HeaderComp/>
    <ConferenceComp/>
  </div>
</template>

<script>
import HeaderComp from './components/HeaderComp.vue'
import ConferenceComp from './components/ConferenceComp.vue'

export default {
  name: 'App',
  components: {
    HeaderComp,
    ConferenceComp
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
</style>
