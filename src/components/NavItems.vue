<template>
  <div class="nav-items">
    <NavItem :link="link" v-for="(link, index) in navItems" :key="index"/>
  </div>
</template>

<script>
import NavItem from "./NavItem.vue";

export default {
    data() {
        return {
            navItems: [
                {text: 'Home', isActive: true},
                {text: 'Find a Doctor', isActive: false},
                {text: 'Apps', isActive: false},
                {text: 'Testimonials', isActive: false},
                {text: 'About Us', isActive: false}
            ]
        }
    },
    components: {
        NavItem,
    },
};
</script>

<style lang="scss" scoped>
.nav-items {
  display: flex;
}
</style>