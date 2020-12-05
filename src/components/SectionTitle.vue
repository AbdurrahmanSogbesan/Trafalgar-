<template>
  <div class="title" :style="{ 'font-size': fontSize }" :class="[textClass]">
    {{ text }}
    <SectionTitleLine v-if="hasLine"/>
  </div>
</template>

<script>
import SectionTitleLine from "./SectionTitleLine.vue";

export default {
  props: {
    text: {
      type: String,
    },
    textClass: {
      type: String,
    },
    fontSize: {
      type: String,
      default: "48px",
    },
    hasLine: {
      type: Boolean,
      default: false,
    },
  },
  components: {
    SectionTitleLine,
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