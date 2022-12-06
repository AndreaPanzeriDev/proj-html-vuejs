<template>
  <div>
    <div class="height">
      <img :src="require(`../../assets/img/${singleItem.img}`)" alt="img" />
      <div class="d-flex italic">
        {{ singleItem.date }}
        /
        {{ singleItem.comments }}
        Comments
      </div>
      <div class="text-black o-7 fw-bold">{{ singleItem.title }}</div>
      <div class="text-black o-5">{{ singleItem.phrase }}</div>
      <a class="italic" href="#">Read More</a>
    </div>
  </div>
</template>

<script>
export default {
  name: "recentNewsCard",
  props: {
    singleItem: Object,
  },
};
</script>

<style scoped>
img {
  width: 100%
}


.height{
  height: 400px;
  position: relative;
}

a {
  color: #f7260c;
  text-decoration: none;
  margin-top: 20px;
  position: absolute;
  bottom: 0;
}
</style>