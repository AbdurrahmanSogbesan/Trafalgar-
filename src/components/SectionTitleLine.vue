<template>
  <div>
    <svg
      width="56"
      height="2"
      viewBox="0 0 56 2"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
    >
      <rect width="56" height="2" rx="1" :fill="color" />
    </svg>
  </div>
</template>

<script>
export default {
  props: {
    color: {
      type: String,
      default: 'black'
    },
  },
};
</script>

<style lang="scss" scoped>
</style>