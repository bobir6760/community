<template>
  <div class="works">
    <div class="container">
      <div class="works-wrapper">
        <div class="works-item__wrapper">
          <div class="works-title">How It Works</div>
          <div class="works-subtitle">
            What our customers <br />
            say about us ?
          </div>
        </div>
        <div class="works-card__wrapper">
          <WorksCard v-for="(card, index) in cards" :key="index" :item="card" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import WorksCard from "@/components/WorksCard";
export default {
  name: "Works",
  data() {
    return {
      cards: [
        {
          imgUrl: require("@/assets/img/ART1.png"),
          title: "Track your savins",
          subtitle: "Track your savings and build better spending habbits ",
        },
        {
          imgUrl: require("@/assets/img/ART1.png"),
          title: "Track your savins",
          subtitle: "Track your savings and build better spending habbits ",
        },
        {
          imgUrl: require("@/assets/img/ART1.png"),
          title: "Track your savins",
          subtitle: "Track your savings and build better spending habbits ",
        },
      ],
    };
  },
  components: {
    WorksCard,
  },
};
</script>

<style lang="scss" scoped>
.works {
  padding: 50px 0px;
}
.works-item__wrapper {
  text-align: center;
}
.works-title {
  color: #5d5fef;
  font-size: 25px;
}
.works-subtitle {
  font-size: 50px;
  font-weight: 900;
}
.works-body {
  text-align: center;
}
.works-wrapper__title {
  font-size: 30px;
  color: #5d5fef;
}
.works-wrapper__subtitle {
  font-size: 50px;
  font-weight: 900;
}
.works-image img {
  width: 100%;
  cursor: pointer;
}
.works-item__wrapper {
  display: flex;
  flex-direction: column;
  gap: 20px;
}
.works-card__wrapper {
  display: flex;
  text-align: center;
  justify-content: space-between;
  font-size: 25px;
}
@media screen and (max-width: 992px) {
  .works-subtitle {
    font-size: 40px;
  }
  .works-item__title {
    font-size: 20px;
  }
  .works-item__subtitle {
    font-size: 18px;
  }
  .works-card__wrapper {
    flex-direction: column;
  }
}
@media screen and (max-width: 768px) {
  .works-subtitle {
    font-size: 30px;
  }
  .works-item__title {
    font-size: 15px;
  }
  .works-item__subtitle {
    font-size: 14px;
  }
}
@media screen and (max-width: 576px) {
  .works-subtitle {
    font-size: 30px;
  }
  .works-item__title {
    font-size: 20px;
  }
  .works-item__subtitle {
    font-size: 18px;
  }
  .works-item {
    flex-direction: column;
  }
}
</style>
