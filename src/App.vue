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
              class="body-margin-bottom"
              text="Trafalgar provides progressive, and affordable healthcare, accessible on mobile and online for everyone. To us, it’s not just work. We take pride in the solutions we deliver"
              bodyFontSize="18px"
            />
            <Button btnClass="outline" text="Learn More" />
          </div>
        </div>
      </section>
      <section class="row download-section">
        <div class="col-5">
          <SectionTitle
            text="Download our mobile apps"
            fontSize="36px"
            hasLine
          />
          <SectionBody
            class="body-margin-bottom"
            text="Our dedicated patient engagement app and web portal allow you to access information instantaneously (no tedeous form, long calls, or administrative hassle) and securely"
            bodyFontSize="18px"
          />
          <Button btnClass="outline" text="Download" :icon="DownloadIcon"/>
        </div>
        <div class="col-7"><DownloadGraphic class="graphic-img"/></div>
      </section>
      <section class="testimonial">
        <TestimonialCard :person="person"/>
      </section>
      <section class="article">
        <SectionTitle text="Check out our latest article" fontSize="36px" hasLine/>
        <ArticleList />
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
import DownloadGraphic from "./components/DownloadGraphic.vue";
import DownloadIcon from "./components/DownloadIcon.vue";
import TestimonialCard from "./components/TestimonialCard.vue";
import ArticleList from "./components/ArticleList.vue";


export default {
  name: "App",
  data() {
    return {
      DownloadIcon,
      person:
        {image: require("@/assets/images/Mask Group.png"),name:"Edward Newgate", title:"Founder Circle", quote: "Our dedicated patient engagement app and web portal allow you to access information instantaneously (no tedeous form, long calls, or administrative hassle) and securely"}
    }
  },
  components: {
    Header,
    SectionGroup,
    IntroSectionGraphic,
    SectionTitle,
    SectionBody,
    ServiceList,
    Button,
    LeadingProvidersGraphic,
    DownloadGraphic,
    TestimonialCard,
    ArticleList
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
.body-margin-bottom {
  margin-bottom: 37px !important;
}
.download-section {
  margin-top: 240px;
}
.testimonial {
  margin-bottom: 216px;
}
.article {
  text-align: center;
}
</style>
