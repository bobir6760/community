<template>
  <div class="navbar">
    <div class="container">
      <div class="navbar-wrapper">
        <div class="navbar-wrapper__title">Re:<span>skale</span></div>
        <div class="navbar-wrapper__subtitle">
          <p>Home</p>
          <p>How it works</p>
          <p>Testimonails</p>
        </div>
        <button class="btn_navbar">Download</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Navbar",
};
</script>

<style lang="scss" scoped>
.navbar {
  padding: 50px 0px;
}
.navbar-wrapper {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.navbar-wrapper__title {
  font-size: 50px;
  font-weight: 900;
  cursor: pointer;
  span {
    color: #5d5fef;
  }
}
.navbar-wrapper__subtitle {
  display: flex;
  font-size: 25px;
  gap: 30px;
  cursor: pointer;
}
.navbar-wrapper__subtitle p {
  color: #5d5fef;
}
.navbar-wrapper__subtitle p:active {
  color: black;
  font-size: 28px;
}
.btn_navbar {
  cursor: pointer;
  padding: 17px 35px;
  border-radius: 12px;
  background: #5d5fef;
  border: none;
  color: white;
  font-size: 18px;
}
.btn_navbar:active {
  color: black;
}
.btn_navbar:hover {
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.9);
}
@media screen and (max-width: 1200px) {
  .navbar-wrapper__subtitle p {
    font-size: 22px;
    gap: 15px;
  }
  .btn_navbar {
    font-size: 15px;
    padding: 15px 30px;
  }
}
@media screen and (max-width: 992px) {
}

@media screen and (max-width: 768px) {
  .navbar-wrapper__subtitle p {
    font-size: 18px;
    gap: 10px;
  }
  .navbar-wrapper__title {
    font-size: 40px;
  }
  .navbar-wrapper__subtitle {
    gap: 15px;
  }
  .btn_navbar {
    font-size: 14px;
    padding: 12px 25px;
  }
}

@media screen and (max-width: 576px) {
  .navbar-wrapper {
    flex-direction: column;
    gap: 30px;
  }
}
</style>
