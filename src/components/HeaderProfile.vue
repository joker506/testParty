<template>
  <div class="header__wrap">
    <div class="header__profile">
      <div class="profile__cash">
        <ul class="cash__items">
          <li class="cash__item">
            R.O.I:
            <span class="item__price">$12,225</span>
          </li>
          <LI class="cash__item">
            Started:
            <span class="item__price">$10,000</span>
          </LI>
          <LI class="cash__item">
            Total Cash:
            <span class="item__price">$12,225</span>
          </LI>
          <LI class="cash__item">
            Invested:
            <span class="item__price">$1,145</span>
          </LI>
          <LI class="cash__item">
            Net Profit:
            <span class="item__price">$2,225</span>
          </LI>
          <LI class="cash__item">
            POT BALANCE:
            <span class="item__price">$235</span>
          </LI>
        </ul>
      </div>
      <div class="profile__cash">
        <img src="~@/assets/2-layers.png" alt />
      </div>
      <div class="profile__status">
        <div class="status__wrapp">
          <table class="status__wrapp">
            <tr>
              <th class="status__item">Won</th>
              <th class="status__item">Lost</th>
              <th class="status__item">In-Play</th>
            </tr>
            <tr>
              <th class="status__item--modif">88</th>
              <th class="status__item--modif">142</th>
              <th class="status__item--modif">2</th>
            </tr>
          </table>
        </div>

        <button class="profile__btn">Edit Profile</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderProfile",
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
  background-image: url(/img/burger.8436f833.svg);
  background-repeat: no-repeat;
  border: none;
  background-color: transparent;
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
    background-image: url(/img/Down_arrow_small.8fc983fd.svg);
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

.header__profile {
  display: flex;
  justify-content: space-between;
}
.profile__cash {
}

.profile__status {
  margin-right: 20px;
}
.status__item {
  color: #ffffff;
  font-family: "Titillium Web";
  font-size: 12px;
  font-weight: 400;
  line-height: 18px;
  margin-top: 0px;
  margin-bottom: 0px;
  &--modif {
    margin-top: 0px;
    margin-bottom: 10px;
    text-shadow: 0 3px 6px rgba(0, 0, 0, 0.3);
    color: #ffffff;
    font-family: "Titillium Web";
    font-size: 16px;
    font-weight: 700;
    line-height: 18px;
  }
}
.cash__items {
  list-style: none;
  margin: 0px;
}
.cash__item {
  height: 14px;
  color: #d9d9d9;
  font-family: "Titillium Web";
  font-size: 8px;
  font-weight: 300;
  line-height: 18px;
  text-transform: uppercase;
  text-align: end;
}
.item__price {
  padding-left: 10px;
  text-shadow: 1px 1px 5px rgba(76, 0, 107, 0.4);
  color: #ebc425;
  font-size: 12px;
  font-weight: 400;
  line-height: 9px;
  font-weight: 600;
}
.status__wrapp {
  // display: flex;
  //justify-content: space-between;
  flex-wrap: wrap;
  width: 121px;
}

.profile__btn {
  width: 121px;
  height: 27px;
  background-color: transparent;
  border-radius: 6px;
  color: #ffffff;
  font-family: "Titillium Web";
  font-size: 8px;
  font-weight: 300;
  line-height: 13px;

  border: 1px solid #ffffff;
}
</style>
