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
  <div class="flex column">
    <img :src="thumb" alt="" />
    <span>{{ series }}</span>
  </div>
</template>

<style lang="scss" scoped>
img {
  width: 6.25rem;
  height: 6.25rem;
}
</style>
