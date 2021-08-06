<template>
  <div class="cover">
    <div class="cover__bg-ellipse">
      <div class="cover__bg-ellipse-items">
        <div class="cover__bg-ellipse-subtitle">
          Добро пожаловать в игру
        </div>
        <div class="cover__bg-ellipse-title">
          Помоги <br />
          <span>Фармацевту</span>
        </div>
        <button class="cover__bg-ellipse-btn">
          <router-link to="/about">Начать</router-link>
        </button>
      </div>
    </div>
    <div class="cover__bg-img">
      <div class="cover__bg"></div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.cover {
  max-width: 100%;
  margin: 0 auto;
  color: #ffff;
  overflow: hidden;

  &__bg-img {
    background: url(../assets/shutterstock_111500834.jpg);
    height: 1000px;
  }

  &__bg {
    height: 1000px;
    background: linear-gradient(63.53deg, #2d8550 16.62%, #5e6ec2 83.38%);
    opacity: 0.35;
  }

  &__bg-ellipse-items {
    display: grid;
    gap: 50px;
    position: relative;
    top: 270px;
    left: 200px;
  }

  &__bg-ellipse-subtitle {
    font-size: 35px;
  }

  &__bg-ellipse-title {
    font-size: 60px;
    font-weight: 600;
  }

  *span {
    font-size: 90px;
  }

  &__bg-ellipse-btn {
    width: 381px;
    height: 90px;

    background: #ffff;
    border-radius: 100px;
    border: none;

    color: #8e9ad5;
    font-size: 36px;

    cursor: pointer;
  }
  *a {
    text-decoration: auto;
  }

  &__bg-ellipse {
    height: 860px;
    width: 860px;

    background: linear-gradient(63.53deg, #2d8550 16.62%, #5e6ec2 83.38%);

    position: absolute;
    z-index: 9999;
    border-radius: 50%;
    left: 110px;
    top: -30px;
  }
}
</style>
