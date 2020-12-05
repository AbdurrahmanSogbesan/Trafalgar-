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
        <div class="col-7"><IntroSectionGraphic class="graphic-img" /></div>
      </section>
      <section class="services">
        <div class="container services">
          <SectionTitle text="Our Services" fontSize="36px" hasLine />
          <SectionBody
            text="We provide to you the best choiches for you. Adjust it to your health needs and make sure your undergo treatment with our highly qualified doctors you can consult with us which type of service is suitable for your health"
            bodyFontSize="18px"
          />
        </div>
      </section>
      <section class="service-list">
        <ServiceList />
      </section>
      <div class="button-center">
        <Button text="Learn More" btnClass="outline" />
      </div>
      <section class="row">
        <div class="col-7">
          <LeadingProvidersGraphic />
        </div>
        <div class="col-5">
          <div class="margin">
            <SectionTitle
              text="Leading healthcare providers"
              fontSize="36px"
              hasLine
            />
            <SectionBody
              text="Trafalgar provides progressive, and affordable healthcare, accessible on mobile and online for everyone. To us, it’s not just work. We take pride in the solutions we deliver"
              bodyFontSize="18px"
            />
          </div>
        </div>
      </section>
    </div>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import SectionGroup from "./components/SectionGroup.vue";
import IntroSectionGraphic from "./components/IntroSectionGraphic.vue";
import SectionTitle from "./components/SectionTitle.vue";
import SectionBody from "./components/SectionBody.vue";
import ServiceList from "./components/ServiceList.vue";
import Button from "./components/Button.vue";
import LeadingProvidersGraphic from "./components/LeadingProvidersGraphic.vue";

export default {
  name: "App",
  components: {
    Header,
    SectionGroup,
    IntroSectionGraphic,
    SectionTitle,
    SectionBody,
    ServiceList,
    Button,
    LeadingProvidersGraphic,
  },
};
</script>

<style lang="scss">
.graphic-img {
  width: 100%;
  margin-left: 80px;
}
.services {
  margin-top: 190px;
  text-align: center;
}
.service-list {
  margin-bottom: 69px;
}
.button-center {
  text-align: center;
  margin-bottom: 221px;
}
.margin {
  margin-left: 50px;
}
</style>
