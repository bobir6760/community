<template>
  <div class="next">
    <div class="container">
      <div class="next-wrapper">
        <div class="next-body">
          <div class="next-card__text">WHAT THEY SAY</div>
          <div class="next-card__subtitle">
            What our customers <br />say about us ?
          </div>
        </div>
        <div class="next-item">
          <div class="next-wrapper__title">
            It was hard to discipline myself in the past.<br />
            The rewards deffinetly help me achieve my goals.
          </div>
          <div class="next-wrapper__subtitle">
            ~ Marry from <span>Canada</span>
          </div>
          <div class="next-wrapper__item">
            <div class="next-wrapper__prev">
              <div class="next-image">
                <img src="@/assets/img/prev.svg" alt="" />
              </div>
              <div class="next-prev__title">Prev</div>
            </div>
            <div class="next-wrapper__block">
              <div class="next-block__title">Next</div>
              <div class="next-image">
                <img src="@/assets/img/next.svg" alt="" />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Next",
};
</script>

<style lang="scss" scoped>
.next {
  padding: 50px 0px;
}
.next-wrapper {
  display: flex;
  flex-direction: column;
  gap: 50px;
}
.next-item {
  display: flex;
  flex-direction: column;
  background-color: #d8d8ff;
  gap: 50px;
  border-radius: 5px;
  padding: 50px 30px 10px 30px;
}
.next-wrapper__title {
  display: flex;
  justify-content: center;
  font-weight: bold;
  font-size: 44px;
  text-align: center;
  align-items: center;
}
.next-wrapper__subtitle {
  font-weight: bold;
  font-size: 30px;
  text-align: center;
  span {
    color: #491cd8;
  }
}
.next-wrapper__prev {
  display: flex;
  align-items: center;
  font-size: 32px;
  gap: 10px;
}
.next-wrapper__block {
  display: flex;
  align-items: center;
  font-size: 32px;
  gap: 10px;
}
.next-wrapper__item {
  display: flex;
  justify-content: space-around;
}
.next-image img {
  width: 100%;
  cursor: pointer;
}
.next-image:active {
  color: white;
}
.next-body {
  text-align: center;
  .next-card__text {
    color: #491cd8;
    font-size: 25px;
    cursor: pointer;
  }
  .next-card__subtitle {
    font-size: 50px;
    font-weight: bold;
  }
}
@media screen and (max-width: 992px) {
  .next-body .next-card__subtitle {
    font-size: 40px;
  }
  .next-wrapper__title {
    font-size: 30px;
  }
  .next-wrapper__subtitle {
    font-size: 20px;
  }
  .next-prev__title {
    font-size: 18px;
  }
  .next-block__title {
    font-size: 18px;
  }
  .next-image img {
    width: 70%;
  }
  .next-image {
    text-align: center;
  }
  .next-wrapper__prev {
    gap: 0px;
  }
  .next-wrapper__block {
    gap: 0px;
  }
}
@media screen and (max-width: 768px) {
  .next-body .next-card__subtitle {
    font-size: 30px;
  }
  .next-body .next-card__text {
    font-size: 20px;
  }
  .next-wrapper__title {
    font-size: 25px;
  }
}
@media screen and (max-width: 576px) {
  .next-wrapper__title {
    font-size: 21px;
  }
  .next-wrapper__subtitle {
    font-size: 18px;
  }
  .next-prev__title {
    font-size: 15px;
  }
  .next-block__title {
    font-size: 15px;
  }
}
</style>
