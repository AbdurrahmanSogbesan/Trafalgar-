<template>
  <div class="body">
    {{ text }}
  </div>
</template>

<script>
export default {
  props: {
    text: {
      type: String,
    },
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
  margin-bottom: 45px;
}
</style>