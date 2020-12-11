<template>
  <div class="header">
    <div class="container d-flex mb-5">
      <Logo />
      <NavItems class="d-md-flex d-none"/>
      <div class="d-md-none d-block toggle">
        <div></div>
        <div></div>
        <div></div>
      </div>
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

.toggle {
  div {
    height: 3px;
    margin-bottom: 4px;
    background-color: black;
    width: 24px;
  }
}
</style>