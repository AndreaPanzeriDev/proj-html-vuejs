<template>
  <div id="card">
    <img :src="require(`../../assets/img/${singleItem}`)" alt="img">
  </div>
</template>

<script>
export default {
    name: 'footerCard',
    props:{
       singleItem: Object 
    }
}
</script>

<style scoped>
#card{
    width: calc(100% / 4 - 5px);
}

img{
    max-width: 100%;
}
</style>