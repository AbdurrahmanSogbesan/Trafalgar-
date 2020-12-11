<template>
  <div class="body" :style="{ 'font-size': bodyFontSize }">
    {{ text }}
  </div>
</template>

<script>
export default {
  props: {
    text: {
      type: String,
    },
    bodyFontSize: {
      type: String,
      default: "21px"
    }
  },
};
</script>

<style lang="scss" scoped>
.body {
  font-weight: 300;
  font-size: 21px;
  line-height: 32px;
  color: #7d7987;
  mix-blend-mode: normal;
  margin-bottom: 80px;
}
</style>