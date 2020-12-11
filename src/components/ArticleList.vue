<template>
  <div class="section">
    <div class="article">
      <ArticleCard
        v-for="(article, index) in articles"
        :key="index"
        :article="article"
      />
    </div>
    <Button btnClass="outline" text="View All" />
  </div>
</template>

<script>
import ArticleCard from "./ArticleCard.vue";
import Button from "./Button.vue";

export default {
  data() {
    return {
      articles: [
        {
          title: "Disease detection, check up in the laboratory",
          body:
            "In this case, the role of the health laboratory is very important to do a disease detection...",
          img: require("@/assets/images/Mask Group (1).png"),
        },
        {
          title: "Herbal medicines that are safe for consumption",
          body:
            "Herbal medicine is very widely used at this time because of its very good for your health...",
          img: require("@/assets/images/Mask Group (2).png"),
        },
        {
          title: "Natural care for healthy facial skin",
          body:
            "A healthy lifestyle should start from now and also for your skin health.There are some...",
          img: require("@/assets/images/Mask Group (3).png")
        },
      ],
    };
  },
  components: {
    ArticleCard,
    Button,
  },
};
</script>

<style lang="scss" scoped>
.section {
  margin-bottom: 201px;
  margin-top: 56px;
}
.article {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  margin-bottom: 69px;
}
</style>