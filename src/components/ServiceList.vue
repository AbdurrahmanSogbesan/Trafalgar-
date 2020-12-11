<template>
  <div class="row">
    <ServiceCard
      v-for="(service, index) in services"
      :key="index"
      :service="service"
    />
  </div>
</template>

<script>
import ServiceCard from "./ServiceCard";
import SearchIcon from "./SearchIcon.vue";
import JarIcon from "./JarIcon.vue";
import ConsultationIcon from "./ConsultationIcon.vue";
import DetailsIcon from "./DetailsIcon.vue";
import EmergencyIcon from "./EmergencyIcon.vue";
import TrackingIcon from "./TrackingIcon.vue";

export default {
  data() {
    return {
      services: [
        {
          title: "Search Doctor",
          body:
            "Choose your doctor from thousands of specialist, general, and trusted hospitals",
          icon: SearchIcon,
        },
        {
          title: "Online Pharmacy",
          body:
            "Buy  your medicines with our mobile application with a simple delivery system",
          icon: TrackingIcon,
        },
        {
          title: "Consultation",
          body:
            "Free consultation with our trusted doctors and get the best recomendations",
          icon: ConsultationIcon,
        },
        {
          title: "Details Info",
          body:
            "Free consultation with our trusted doctors and get the best recomendations",
          icon: DetailsIcon,
        },
        {
          title: "Emergency Care",
          body:
            "Free consultation with our trusted doctors and get the best recomendations",
          icon: EmergencyIcon,
        },
        {
          title: "Tracking",
          body: "Track and save your medical history and health data",
          icon: JarIcon,
        },
      ],
    };
  },
  components: {
    ServiceCard,
  },
};
</script>

<style lang="scss" scoped>
</style>