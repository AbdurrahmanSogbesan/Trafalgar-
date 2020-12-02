<template>
  <div class="title">
    {{ text }}
  </div>
</template>

<script>
export default {
  props: {
    text: {
      type: String,
    },
    // fontSize: {
    //   type: Number + "px",
    // },
  },
};
</script>

<style lang="scss" scoped>
.title {
  font-weight: bold;
  font-size: 48px;
  line-height: 56px;
  color: #000000;
  margin-bottom: 25px;
}
</style>