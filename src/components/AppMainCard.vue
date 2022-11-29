<script>
export default {
  name: "AppMainCard",
  props: {
    thumb: "",
    series: "",
  },
};
</script>

<template>
  <div class="flex column align-items-center margin-1">
    <img :src="thumb" alt="" />
    <span>{{ series }}</span>
  </div>
</template>

<style lang="scss" scoped>
.margin-1 {
  margin-top: 0.625rem;
}
img {
  width: 6.25rem;
  height: 6.25rem;
}
</style>
