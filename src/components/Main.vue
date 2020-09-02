<template>
  <div class>
    <div class="main__wrap">
      <div class="main__menu">MY BETS</div>
      <div v-bind:class="{ active: isActive }" class="main__menu--mod">MY EFFICIENCY</div>
    </div>

    <div class="main__nav">
      <div class="nav__item--calendar">DEC-JAN</div>
      <div class="nav__item">Time</div>
      <div class="nav__item">
        H/D/A
        <br />Y / N
      </div>
      <div class="nav__item">Market</div>
      <div class="nav__item leag">League</div>
      <div class="nav__item">
        Price
        %
      </div>
      <div class="nav__item">
        Stake
        <br />W / L
      </div>
    </div>

    <div class="main__section">
      <div v-for="(item) in users" :key="item.id" class="section__item">
        <div class="section__param calend">
          <table class>
            <tr>
              <td>1</td>
              <td style="text-align: left">Inter Milan</td>
            </tr>
            <tr>
              <td>2</td>
              <td>S.S.C Napoli</td>
            </tr>
          </table>
        </div>
        <div class="section__param clock">14:00</div>
        <div class="section__param letter">H</div>
        <div class="section__param market">BTS</div>
        <div class="section__param leage">Champ LE</div>
        <div class="section__param calend">
          <table class>
            <tr>
              <td style="color: #c2c2c2;">2.1</td>
            </tr>
            <tr>
              <td>11.5%</td>
            </tr>
          </table>
        </div>
        <div class="section__param calend">
          <table class>
            <tr>
              <td style="color: #ebc425;">$ 100</td>
            </tr>
            <tr>
              <td style="color: #1aff00;">$ 150</td>
            </tr>
          </table>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Main",
  data() {
    return {
      users: [{ id: 0 }, { id: 1 }, { id: 2 }, { id: 3 }],
      isActive: false,
    };
  },
};
</script>

<style lang="scss" scoped>
.active {
  font-style: italic;
}
.main__wrap {
  margin-top: 25px;
  margin-bottom: 17px;
  display: flex;
  justify-content: space-between;
  border-bottom: 1px solid #979797;
  opacity: 0.8;
}
.main__menu {
  width: 200px;
  text-shadow: 0 3px 6px rgba(0, 0, 0, 0.2);
  color: #ffffff;
  font-family: "Titillium Web", sans-serif;
  font-size: 16px;
  font-weight: 600;
  line-height: 18px;
  text-transform: uppercase;
  border-bottom: 3px solid #ee3696;
}
.main__menu--mod {
  width: 200px;
  opacity: 0.75;
  text-shadow: 0 3px 6px rgba(0, 0, 0, 0.2);
  color: #ffffff;
  font-family: "Titillium Web", sans-serif;
  font-size: 16px;
  font-weight: 300;
  line-height: 18px;
  text-transform: uppercase;
  border-bottom: 3px solid transparent;
}
.main__nav {
  display: flex;
  // height: 51px;
  box-shadow: 3px 11px 8px rgba(0, 0, 0, 0.5);
  border-radius: 10px;
  background-image: linear-gradient(
    to top,
    rgba(150, 112, 167, 0.51) 0%,
    #ff0080 100%
  );

  margin-bottom: 5px;
}
.nav__item {
  color: #ffffff;
  box-sizing: border-box;
  font-family: "Titillium Web", sans-serif;
  font-size: 10px;
  font-weight: 400;
  line-height: 12px;
  text-transform: capitalize;
  padding: 7px;
  padding-top: 12px;
  border-right: 1px solid #f3cde0;
  opacity: 0.7;
  &:hover {
    opacity: 1;
  }
}
.leag {
  width: 58px;
}

.nav__item--calendar {
  box-sizing: border-box;
  width: 112px;
  color: #ffffff;
  font-family: "Titillium Web", sans-serif;
  font-size: 10px;
  font-weight: 400;
  line-height: 9px;
  text-transform: uppercase;
  padding-top: 12px;
  padding-left: 26px;
  border-right: 1px solid #f3cde0;
  position: relative;
  opacity: 0.7;
  &:hover {
    opacity: 1;
  }
  &::before {
    content: "";
    position: absolute;
    top: 12px;
    left: 12px;
    background-image: url("~@/assets/calendar.png");
    width: 29px;
    height: 29px;
  }
}
.nav__item:nth-child(2) {
  width: 41px;
  position: relative;
  text-transform: capitalize;
  &::before {
    content: "";
    position: absolute;
    top: 28px;
    left: 15px;
    width: 7px;
    height: 7px;
    background-image: url("~@/assets/Path_10.svg");
  }
}
.nav__item:last-child {
  border-right: none;
  box-sizing: border-box;
}

.section__item {
  width: 373px;
  height: 50px;
  display: flex;
  justify-content: space-around;
  margin: 5px auto;
  border-radius: 5px;
  opacity: 0.8;
  background-image: url("~@/assets/HIstoryBck01.png");
}
.section__param {
  color: #ffffff;
  font-family: "Titillium Web", sans-serif;
  font-size: 12px;
  font-weight: 400;
}
.calend {
  margin-top: 5px;
}

.clock {
  width: 41px;
  font-size: 8px;
  font-weight: 300;
  letter-spacing: 0.34px;
  line-height: 14px;
  margin-top: 15px;
}
.letter {
  font-size: 12px;
  font-weight: 400;
  line-height: 14px;
  margin-top: 15px;
  margin-left: 5px;
  margin-right: 5px;
}
.market {
  margin-top: 15px;
  margin-left: 15px;
}
.leage {
  width: 58px;
  font-size: 11px;
  margin-top: 15px;
  line-height: 14px;
  font-style: italic;
}
</style>
