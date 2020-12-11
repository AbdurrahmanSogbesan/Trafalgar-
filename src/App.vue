<template>
  <div id="app">
    <Header />
    <div class="container">
      <section class="intro-section row align-items-center">
        <div class="col-md-5 col-12">
          <SectionGroup
            title="Virtual healthcare for you"
            body="Trafalgar provides progressive, and affordable healthcare, accessible on mobile and online for everyone"
            :buttonProps="{ text: 'Consult Today' }"
          />
        </div>
        <div class="col-md-7 col-12"><IntroSectionGraphic class="graphic-img" /></div>
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
        <div class="col-md-7 col-12">
          <LeadingProvidersGraphic class="mb-5"/>
        </div>
        <div class="col-md-5 col-12">
          <div class="margin">
            <SectionTitle text="Leading healthcare providers" fontSize="36px" hasLine />
            <SectionBody
              class="body-margin-bottom"
              text="Trafalgar provides progressive, and affordable healthcare, accessible on mobile and online for everyone. To us, it’s not just work. We take pride in the solutions we deliver"
              bodyFontSize="18px"
            />
            <Button btnClass="outline" text="Learn More" wrapperClass="text-resp" />
          </div>
        </div>
      </section>
      <section class="row download-section">
        <div class="col-md-5 col-12">
          <SectionTitle text="Download our mobile apps" fontSize="36px" hasLine />
          <SectionBody
            class="body-margin-bottom"
            text="Our dedicated patient engagement app and web portal allow you to access information instantaneously (no tedeous form, long calls, or administrative hassle) and securely"
            bodyFontSize="18px"
          />
          <Button btnClass="outline" text="Download" :icon="DownloadIcon" wrapperClass="text-resp"/>
        </div>
        <div class="col-md-7 col-12"><DownloadGraphic class="graphic-img" /></div>
      </section>
      <section>
        <TestimonialCard :person="person" />
      </section>
      <section class="article">
        <SectionTitle text="Check out our latest article" fontSize="36px" hasLine />
        <ArticleList />
      </section>
    </div>
    <section>
      <Footer />
    </section>
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
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  data() {
    return {
      DownloadIcon,
      person: {
        image: require("@/assets/images/Mask Group.png"),
        name: "Edward Newgate",
        title: "Founder Circle",
        quote:
          "Our dedicated patient engagement app and web portal allow you to access information instantaneously (no tedeous form, long calls, or administrative hassle) and securely",
      },
    };
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
    ArticleList,
    Footer,
  },
};
</script>

<style lang="scss">
.graphic-img {
  width: 100%;
  margin-left: 80px;

  @media (max-width: 480px) {
    margin-left: 0;
    margin-top: 60px;
  }
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

  @media (max-width: 480px) {
    margin-bottom: 100px;
  }
}
.margin {
  margin-left: 50px;

  @media (max-width: 480px) {
    margin-left: 0;
  }
}
.body-margin-bottom {
  margin-bottom: 37px !important;
}
.download-section {
  margin-top: 240px;

  @media(max-width: 480px){
      margin-top: 100px;
    }
}
.article {
  text-align: center;

}
</style>
