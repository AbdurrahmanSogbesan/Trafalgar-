<template>
  <div class="title" :style="{ 'font-size': fontSize, 'color': color }" :class="[textClass]">
    {{ text }}
    <SectionTitleLine :color="lineColor" v-if="hasLine"/>
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
    color: {
      type: String,
      default: "black",
    },
    hasLine: {
      type: Boolean,
      default: false,
    },
    lineColor: {
      type: String,
      default: 'black'
    }
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

  @media (max-width: 480px) {
    text-align: center;
  }
}
</style>