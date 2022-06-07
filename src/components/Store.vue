<template>
  <div class="store">
    <div class="container">
      <div class="store-wrapper">
        <div class="store-item__wrapper">
          <div class="store-wrapper__title">
            Earning rewards <br />has never been <br />so easy
          </div>
          <div class="store-block">
            <div class="store-card__wrapper">
              <div class="store-card__image">
                <img src="@/assets/img/apple.svg" alt="" />
              </div>
              <div class="store-card__block">
                <div class="store-card__title">Download on the</div>
                <div class="store-card__subtitle">app store</div>
              </div>
            </div>
            <div class="store-body__wrapper">
              <div class="store-card__image">
                <img src="@/assets/img/Play.svg" alt="" />
              </div>
              <div class="store-card__block">
                <div class="store-card__title">Download on the</div>
                <div class="store-card__subtitle">app store</div>
              </div>
            </div>
          </div>
        </div>
        <div class="store-image">
          <img src="@/assets/img/iPhone.png" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Store",
};
</script>

<style lang="scss" scoped>
.store {
  padding: 50px 0px;
}
.store-wrapper {
  display: flex;
  background-color: #5d5fef;
  border-radius: 20px;
  padding: 30px;
  align-items: center;
}
.store-item__wrapper {
  flex: 1;
  display: flex;
  flex-direction: column;
  gap: 20px;
}
.store-wrapper__title {
  font-size: 70px;
  color: white;
  font-weight: 900;
  font-weight: bold;
}
.store-block {
  display: flex;
  gap: 50px;
}
.store-card__wrapper {
  display: flex;
  gap: 10px;
  align-items: center;
  color: #fff;
  background-color: #491cd8;
  padding: 5px 50px 5px 5px;
  border-radius: 10px;
  text-align: center;
  cursor: pointer;
}
.store-card__wrapper:active {
  color: aqua;
}
.store-card__wrapper:hover {
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.9);
}
.store-body__wrapper {
  display: flex;
  gap: 10px;
  align-items: center;
  color: #fff;
  background-color: #491cd8;
  padding: 5px 50px 5px 5px;
  border-radius: 10px;
  text-align: center;
  cursor: pointer;
}
.store-body__wrapper:active {
  color: aqua;
}
.store-body__wrapper:hover {
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.9);
}
.store-card__subtitle {
  font-weight: bold;
  font-size: 16px;
}
.store-image img {
  flex: 1;
  width: 100%;
}
.store-card__image img {
  object-fit: contain;
  width: 60px;
  height: 60px;
}
@media screen and (max-width: 1200px) {
  .store-wrapper__title {
    font-size: 50px;
  }
}
@media screen and (max-width: 992px) {
  .store-wrapper__title {
    font-size: 40px;
  }
  .store-image img {
    width: 100%;
  }
  .store-card__image img {
    width: 40px;
    height: 40px;
  }
  .store-block {
    gap: 10px;
  }
  .store-wrapper {
    padding: 10px;
  }
  .store-card__title {
    font-size: 16px;
  }
  .store-body__wrapper {
    padding: 5px 30px 5px 5px;
  }
  .store-card__wrapper {
    padding: 5px 30px 5px 5px;
  }
}
@media screen and (max-width: 768px) {
  .store-wrapper__title {
    font-size: 30px;
  }
  .store-image {
    display: none;
  }
  .store-item__wrapper {
    gap: 30px;
    text-align: center;
  }
  .store-block {
    gap: 30px;
    justify-content: center;
  }
}
@media screen and (max-width: 576px) {
  .store-image {
    display: block;
  }
  .store-block {
    display: flex;
    flex-direction: column;
  }
  .store-body__wrapper {
    display: flex;
    justify-content: center;
  }
  .store-card__wrapper {
    display: flex;
    justify-content: center;
  }
  .store-wrapper {
    flex-direction: column;
    gap: 30px;
  }
}
</style>
