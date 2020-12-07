<template>
  <div class="testimonial">
    <SectionTitle
      text="What are our customers saying?"
      fontSize="36px"
      color="white"
      hasLine
      lineColor="white"
      class="title"
    />
    <div class="testimonial-body">
      <TestimonialPerson name="Edward Newgate" title="Founder Circle"/>
      <div class="testimonial-text">
        “Our dedicated patient engagement app and web portal allow you to access
        information instantaneously (no tedeous form, long calls, or
        administrative hassle) and securely”
      </div>
    </div>
  </div>
</template>

<script>
import SectionTitle from "./SectionTitle.vue";
import TestimonialPerson from "./TestimonialPerson.vue";

export default {
  components: {
    SectionTitle,
    TestimonialPerson,
  },
};
</script>

<style lang="scss" scoped>
.testimonial {
  margin-top: 266px;
  width: 1120px;
  height: 425px;
  background: linear-gradient(208.18deg, #67c3f3 9.05%, #5a98f2 76.74%);
  border-radius: 24px;
  padding: 64px 118px 79px 118px;
  text-align: center;
}
.title {
    margin-bottom: 45px !important;
}
.testimonial-body {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
}
.testimonial-text {
  font-size: 19px;
  line-height: 30px;
  color: rgba(255, 255, 255, 0.9);
  max-width: 420px;
  text-align: left;
}
</style>