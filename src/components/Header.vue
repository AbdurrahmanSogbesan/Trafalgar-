<template>
  <div class="header">
    <div class="container d-flex">
      <Logo />
      <NavItems />
    </div>
  </div>
</template>

<script>
import Logo from "./Logo.vue";
import NavItems from "./NavItems.vue";

export default {
  components: {
    Logo,
    NavItems,
  },
};
</script>

<style lang="scss" scoped>
.header {
    padding-top: 56px;
  .container {
    justify-content: space-between;
    align-items: center;
  }
}
</style>