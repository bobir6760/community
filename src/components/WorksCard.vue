<template>
  <div class="works-item">
    <div class="works-item__wrapper">
      <div class="works-image">
        <img :src="item.imgUrl" alt="" />
      </div>
      <div class="works-item__title">{{ item.title }}</div>
      <div class="works-item__subtitle">
        {{ item.subtitle }}
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "works-card",
  props: {
    item: {
      type: Object,
      required: true,
    },
  },
};
</script>

<style scoped lang="scss">
.works-item__wrapper {
  display: flex;
  flex-direction: column;
  gap: 10px;
  .works-item__title {
    font-weight: bold;
    cursor: pointer;
  }
  .works-image {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .works-image img {
    cursor: pointer;
    width: 80%;
  }
}
@media screen and (max-width: 992px) {
  .works-item__wrapper {
    display: flex;
    flex-direction: column;
    text-align: center;
  }
}
@media screen and (max-width: 576px) {
  .works-image {
    align-items: center;
  }
}
</style>
