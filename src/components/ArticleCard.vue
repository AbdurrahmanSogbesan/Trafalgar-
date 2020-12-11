<template>
  <div class="article-card mb-md-0 mb-5" >
    <img :src="article.img" />
    <div class="article-text">
      <div class="article-title">
        {{ article.title }}
      </div>
      <div class="article-body">
        {{ article.body }}
      </div>
      <ReadMore />
    </div>
  </div>
</template>

<script>
import ReadMore from "./ReadMore.vue";

export default {
  props: {
    article: {
      type: Object,
    },
  },
  components: {
    ReadMore,
  },
};
</script>

<style lang="scss" scoped>
.article-card {
  width: 350px;
  height: 512px;
  background: #FFF;
  box-shadow: 10px 40px 50px rgba(229, 233, 246, 0.4);
  border-radius: 20px;
  text-align: left;
}
.article-text {
  padding: 24px 51px 35px 33px;
}

.article-title {
  font-weight: bold;
  font-size: 21px;
  line-height: 32px;
  color: #000000;
  margin-bottom: 12px;
}
.article-body {
  font-weight: 300;
  font-size: 16px;
  line-height: 28px;
  color: #7d7987;
  margin-bottom: 25px;
}
</style>