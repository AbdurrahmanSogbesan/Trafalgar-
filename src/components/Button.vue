<template>
  <div>
    <button class="button" :class="[btnClass]">{{ text }}</button>
  </div>
</template>

<script>
export default {
  props: {
    text: {
      type: String,
    }, btnClass: {
        type: String,
        default: ''
    }
  },
};
</script>

<style lang="scss" scoped>
.button {
  height: 60px;
  width: 200px;
  border-radius: 55px;
  background-color: #458ff6;
  border: 1.4px solid #458ff6;
  color: #fff;
  font-weight: bold;
  font-size: 18px;
  box-sizing: border-box;
}

.button.outline {
  background-color: white;
  color: #458ff6;
}
</style>