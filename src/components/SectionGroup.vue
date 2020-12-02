<template>
  <div>
    <SectionTitle :text="title" />
    <SectionBody :text="body" />
    <Button :text="buttonProps.text" :btnClass="buttonProps.btnClass" />
  </div>
</template>

<script>
import SectionTitle from "./SectionTitle.vue";
import SectionBody from "./SectionBody.vue";
import Button from "./Button.vue";

export default {
  components: {
    SectionTitle,
    SectionBody,
    Button,
  },
  props: {
    title: {
      type: String,
    },
    body: String,
    buttonProps: {
      type: Object,
    },
  },
};
</script>

<style lang="scss" scoped>
</style>