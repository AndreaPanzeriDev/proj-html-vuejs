<template>
  <div>
    <div class="icon"><i :class="`${singleItem.icon} fs-2`"></i></div>
    <div class="equal">
      <h4 class="title text-black">{{ singleItem.title }}</h4>
      <p class="phrase">
        {{ singleItem.phrase }}
      </p>
      <a class="italic" href="#">Learn More</a>
    </div>
  </div>
</template>

<script>
export default {
  name: "QuestionCard",
  props: {
    singleItem: Object,
  },
};
</script>

<style scoped>

.title {
  font-weight: 400;
}

.phrase{
    font-weight: lighter;
}
.icon {
  margin-top: 15px;
  margin-right: 10px;
}

a{
    color: #f7260c;
    text-decoration: none;
    margin-top: 20px;
    position: absolute;
    bottom: 0;
}

.equal{
    position: relative;
}
</style>







