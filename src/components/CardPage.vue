<template>
  <div class="col">
    <div class="contents p-4">
      <img class="img-fluid" :src="album.poster" :alt="album.title" />
      <h2 class="title text-white text-center mt-4 mb-3 text-uppercase fs-5">
        {{ album.title }}
      </h2>
      <span class="author d-block text-center fs-6">{{ album.author }}</span>
      <span class="year d-block text-center fs-6">{{ album.year }}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardPage",
  props: {
    album: Object,
  },
};
</script>

<style lang="scss" scoped>
.contents {
  height: 100%;
  background-color: #2e3a46;
}
.author,
.year {
  color: #82766a;
}
</style>
