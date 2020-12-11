<template>
  <div>
    <SectionTitle :text="title" :textClass="textClass" :fontSize="titleFontSize" :hasLine="titleHasLine"/>
    <SectionBody :text="body" :bodyFontSize="bodyFontSize"/>
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
    textClass: {
      type: String,
      default: ''
    },
    titleFontSize:{
      type: String,
      default: '48px'
    }, 
    titleHasLine: {
      type: Boolean,
      default: false
    },
    bodyFontSize: {
      type: String,
      default: '21px'
    }
  },
};
</script>

<style lang="scss" scoped>
</style>