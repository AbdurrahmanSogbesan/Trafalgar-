<template>
  <div class="mr-4 nav-item" :class="{bold: link.isActive}">
    {{ link.text }}
  </div>
</template>

<script>
export default {
  props: {
    link: {
      type: Object, //* {text: '', isActive: true}
    },
  },
};
</script>

<style lang="scss" scoped>
.nav-item {
  font-size: 18px;
  line-height: 23px;
  color: #1f1534;
  opacity: 0.5;
}
.nav-item.bold {
  color: #1f1534;
  font-weight: bold;
  opacity: 1;
}
</style>