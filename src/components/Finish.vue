<template>
  <div class="finish">
    <div class="container">
      <div class="finish-wrapper">
        <div class="finish-title">
          Join our mission to <br />empower women to save
        </div>
        <div class="finish-btn">
          <button class="btn-finish">
            <img src="@/assets/img/apple.svg" alt="" /> Download on the app
            store
          </button>
          <button class="btn-finish">
            <img src="@/assets/img/Play.svg" alt="" /> Download on the app store
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Finish",
};
</script>

<style lang="scss" scoped>
.finish {
  padding: 50px 0px;
}
.finish-wrapper {
  display: flex;
  align-items: center;
  justify-content: space-between;
  font-weight: 900;
  background-color: #a5a6f6;
  border-radius: 10px;
  padding: 40px;
}
.finish-title {
  font-size: 45px;
}
.finish-btn {
  display: flex;
  flex-direction: column;
  gap: 20px;
}
.btn-finish {
  display: flex;
  background-color: #491cd8;
  color: white;
  font-size: 20px;
  border-radius: 10px;
  border: none;
  padding: 10px 20px 10px 10px;
  align-items: center;
  gap: 10px;
  cursor: pointer;
}
.btn-finish:active {
  color: greenyellow;
}
.btn-finish:hover {
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.9);
}
.btn-finish img {
  object-fit: contain;
  width: 50px;
  height: 50px;
}
@media screen and (max-width: 992px) {
  .finish-title {
    font-size: 38px;
  }
  .btn-finish {
    display: flex;
    background-color: #491cd8;
    color: white;
    font-size: 15px;
    border-radius: 10px;
    border: none;
    padding: 10px;
    gap: 0px;
    cursor: pointer;
  }
  .btn-finish img {
    object-fit: contain;
    width: 30px;
    height: 30px;
  }
}
@media screen and (max-width: 768px) {
  .finish-title {
    font-size: 30px;
  }
  .btn-finish {
    font-size: 10px;
  }
  .finish-wrapper {
    padding: 20px;
  }
}
@media screen and (max-width: 576px) {
  .finish-wrapper {
    flex-direction: column;
    gap: 30px;
    text-align: center;
  }
}
</style>
