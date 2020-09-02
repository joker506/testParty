<template>
  <div class="header__wrap">
    <div class="header__top">
      <button class="burger__btn"></button>
      <div class="header__top--balance">
        <div class="balance__wrap">
          <p class="balance__money">$12,225</p>
          <p class="balance__pot">
            MY POT BALANCE:
            <span style="color:#1aff00;">$235</span>
          </p>
        </div>
        <img class="balance__img" src="~@/assets/smile-1726471_960_720.png" alt />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderTop",
};
</script>

<style lang="scss" scoped>
.header__top {
  display: flex;
  justify-content: space-between;
  margin-bottom: 30px;
}

.burger__btn {
  width: 17px;
  height: 15px;
  margin-top: 31px;
  margin-left: 24px;
  background-image: url("~@/assets/burger.svg");
  background-repeat: no-repeat;
  border: none;
  background-color: transparent;
  cursor: pointer;
}
.header__top--balance {
  display: flex;
  margin-right: 15px;
}
.balance__money {
  margin-bottom: 0px;
  margin-top: 23px;
  text-shadow: 0 0 5px rgba(255, 236, 62, 0.65);
  color: #ebc425;
  font-size: 18px;
  font-weight: 600;
  line-height: 9px;
  text-align: end;
  font-family: "Titillium Web - Regular";
  font-weight: 400;
  position: relative;
  &::before {
    content: "";
    position: absolute;
    left: 38px;
    top: 3px;
    width: 10px;
    height: 7px;
    background-image: url("~@/assets/Down_arrow_small.svg");
    background-repeat: no-repeat;
  }
}
.balance__pot {
  opacity: 0.75;
  color: #ffffff;
  font-size: 10px;
  font-weight: 300;
  letter-spacing: 0.1px;
  line-height: 9px;
  text-transform: uppercase;
  font-family: "Titillium Web - Regular";
  font-weight: 400;
}
.balance__img {
  width: 28px;
  height: 28px;
  margin-top: 24px;
  margin-right: 15px;
}
</style>
