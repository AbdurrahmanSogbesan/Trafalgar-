<template>
  <div id="app">
    <Header />
    <div class="container">
      <section class="intro-section row align-items-center">
        <div class="col-5">
          <SectionGroup
            title="Virtual healthcare for you" 
            body="Trafalgar provides progressive, and affordable healthcare, accessible on mobile and online for everyone"
            :buttonProps="{ text: 'Consult Today' }"
          />
        </div>
        <div class="col-7"><IntroSectionGraphic /></div>
      </section>
    </div>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import SectionGroup from "./components/SectionGroup.vue";
import IntroSectionGraphic from "./components/IntroSectionGraphic.vue";

export default {
  name: "App",
  components: {
    Header,
    SectionGroup,
    IntroSectionGraphic,
  },
};
</script>

<style lang="scss">
</style>
