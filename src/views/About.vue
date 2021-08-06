<template>
  <div class="menu">
    <div class="menu__items">
      <div class="menu__btns">
        <button class="menu__btn">
          <img src="../assets/icons/btn_home.png" alt="" />
        </button>
        <button class="menu__btn">
          <img src="../assets/icons/btn_retry.png" alt="" />
        </button>
      </div>
      <div class="menu__counters">
        <div class="menu__counters-title">Параметри:</div>
        <div class="menu__counters-items">
          <div class="menu__counters-item">
            <img src="../assets/icons/sad_icon.png" alt="" />
            {{ sad }}
          </div>
          <div class="menu__counters-item">
            <img src="../assets/icons/happy_icon.png" alt="" />
            {{ happy }}
          </div>
          <div class="menu__counters-item">
            <img src="../assets/icons/heart_icon.png" alt="" />
            {{ heart }}
          </div>
        </div>
      </div>
      <div class="menu__slides">
        <div class="menu__slides-title">Осталось в очереди:</div>
        <div class="menu__slides-counter">14/15</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      sad: 1,
      happy: 2,
      heart: 3,
    };
  },
};
</script>

<style lang="scss">
.menu {
  width: 470px;
  height: 1024px;
  color: #ffff;
  font-size: 36px;

  background: linear-gradient(63.53deg, #2d8550 16.62%, #5e6ec2 83.38%);
  opacity: 0.7;

  &__items {
    display: grid;
    grid-template-rows: 430px 460px 134px;
  }

  &__btn {
    border-radius: 50%;
    border: none;
  }

  &__counters-title {
    font-weight: 600;
  }

  &__counters-items {
    display: grid;
    grid-template-columns: 50% 50%;
    grid-template-rows: 100px 100px;
  }

  &__counters-item:nth-child(3) {
    grid-column: 1/4;

    justify-self: center;
  }

  &__counters-item {
    font-size: 48px;
    color: #424242;

    width: 190px;
    height: 80px;
    background: #ffff;
    border-radius: 40px;
    box-shadow: 0px 0px 50px rgb(131 42 64 / 40%);

    display: grid;
    grid-template-columns: 50% 50%;
    justify-items: center;
    align-items: center;
  }
}
</style>
