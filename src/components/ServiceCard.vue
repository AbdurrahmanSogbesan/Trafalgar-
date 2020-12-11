<template>
  <div class="col-md-4 col-12 service-container">
    <div class="service-card">
    <component class="component-padding" :is="service.icon"> </component>
    <div class="title">{{ service.title }}</div>
    <div class="body">{{ service.body }}</div>
    </div>
   
  </div>
</template>

<script>


export default {
  props: {
    service: {
      type: Object
    }
  },
};
</script>

<style lang="scss" scoped>
.service-container{
  padding-bottom: 30px;
}
.service-card {
  width: 100%;
  height: 354px;
  background: #ffffff;
  box-shadow: 10px 40px 50px rgba(229, 233, 246, 0.4);
  border-radius: 20px;
  padding: 54px 45px 46px 39px;
  display: flex;
  flex-direction: column;
}

.component-padding {
  padding-bottom: 25px;
}

.title {
  font-weight: bold;
  font-size: 24px;
  line-height: 56px ;
  color: #000000;
}

.body {
  font-weight: 300;
  font-size: 16px;
  line-height: 28px;
  color: #7d7987;
}
</style>