<template>
  <div class="person align-items-center">
    <img :src="person.image" class="image" />
    <div class="person-details">
      <div class="name">{{ person.name }}</div>
      <div class="title">{{ person.title }}</div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    person: Object
  },
};
</script>

<style lang="scss" scoped>
.person {
  display: flex;
  flex-direction: row;
}

.image {
  border: 4px solid white;
  border-radius: 80px;
}
.person-details {
    text-align: left;
    margin-left: 29px;
}
.name {
  font-size: 22px;
  font-weight: bold;
  color: #ffffff;
}
.title {
  font-size: 18px;
  line-height: 48px;
  color: rgba(255, 255, 255, 0.85);
}
</style>