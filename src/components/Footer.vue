<template>
  <div class="footer">
    <h3 class="footer__title">Today</h3>
    <div class="footer__top">
      <table class="footer__table">
        <tr>
          <td class="table__heading">Total Bets</td>
          <td class="table__heading">Total Loss</td>
          <td class="table__heading">Total Won</td>
          <td class="table__heading">Net P&L</td>
          <td class="table__heading">R.O.I</td>
        </tr>
        <tr>
          <td class="table__price">$ 800</td>
          <td class="table__price">$ 400</td>
          <td class="table__price">$ 900</td>
          <td class="table__price">$ 500</td>
          <td class="table__price">$ 500</td>
        </tr>
        <tr>
          <td>8</td>
          <td>4</td>
          <td>3</td>
        </tr>
      </table>
      <div class="footer__nav">
        <ul class="nav__items">
          <li class="nav__item house">
            <a href="#">HOME</a>
          </li>
          <li class="nav__item match">
            <a href="#">MATCHES</a>
          </li>
          <li class="nav__item proff">
            <a href="#">PROFILE</a>
          </li>
          <li class="nav__item notif">
            <a href="#">NOTIFICATIONS</a>
          </li>
          <li class="nav__item educat">
            <a href="#">EDUCATION</a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style lang="scss" scoped>
.footer__title {
  color: #ffffff;
  font-family: "Titillium Web", sans-serif;
  font-size: 8px;
  font-weight: 400;
  line-height: 14px;
  height: 14px;
  background-color: black;
  margin-bottom: 0px;
}
.footer__top {
  // background-color: #000000;
  //box-shadow: 0 3px 6px rgba(0, 0, 0, 0.5);
  //opacity: 0.65;
  background-image: linear-gradient(
    180deg,
    rgba(0, 0, 0, 0) 0%,
    rgba(0, 0, 0, 0.05) 12%,
    rgba(0, 0, 0, 0.87) 66%,
    #000000 100%
  );
}

.footer__table {
  padding-top: 10px;
  margin: 0 auto;
  color: #ffffff;
  font-family: "Titillium Web", sans-serif;
  font-size: 14px;
  font-weight: 400;
  line-height: 14px;
  position: relative;
}
.table__heading {
  width: 53px;
  opacity: 0.5;
  color: #ffffff;
  font-family: "Titillium Web", sans-serif;
  font-size: 10px;
  font-weight: 400;
  line-height: 14px;
}
.table__price {
  color: #ffffff;
  font-size: 14px;
  font-weight: 600;
  line-height: 14px;
  font-family: "Titillium Web - Bold";
  font-weight: 700;
}

.footer__nav {
  padding-top: 50px;
  font-family: "Titillium Web";
  font-size: 10px;
  font-weight: 300;
  letter-spacing: 0.1px;
  line-height: 9px;
  padding-bottom: 10px;
  background-image: linear-gradient(
    180deg,
    rgba(0, 0, 0, 0) 0%,
    rgba(0, 0, 0, 0.05) 12%,
    rgba(0, 0, 0, 0.87) 66%,
    #000000 100%
  );
  cursor: pointer;
}
.nav__items {
  display: flex;
  justify-content: space-around;
  list-style: none;
  padding: 0;
  font-family: "Titillium Web";
  font-size: 10px;
  font-weight: 300;
}

.house,
.match,
.proff,
.notif,
.educat {
  color: #ffffff;
  position: relative;
  &::before {
    content: "";
    display: block;
    width: 20px;
    height: 20px;
    position: absolute;
    bottom: 10px;
    left: 3px;
    background-size: contain;
    background-repeat: no-repeat;
  }
}
.house::before {
  background-image: url("~@/assets/baseline_home_white_36dp.svg");
}
.match::before {
  left: 12px;
  background-image: url("~@/assets/Path_2057.svg");
}
.proff::before {
  bottom: 12px;
  left: 9px;
  background-image: url("~@/assets/User.svg");
}
.notif::before {
  bottom: 11px;
  left: 25px;
  background-image: url("~@/assets/Path.svg");
}
.educat::before {
  left: 15px;
  background-image: url("~@/assets/Education.svg");
}
.nav__item > a {
  color: #ffffff;
  text-decoration: none;
}
</style>
