<template>
  <header class="header">
    <div class="header__container">
      <img class="header__container-logo" src="@/assets/images/LocoCompany.svg" alt="">
      <a class="header__container-phone" href="">+7 987 654 32-10</a>
    </div>
  </header>
</template>

<script>

export default {
  name: 'TheHeader',
  props: {
    name: {
      type: String,
      default: ''
    }
  },
  setup () {
  }
}
</script>

<style lang="css" scoped>
.header {
  background-color: blue;
  padding: 13px;

  &__container {
    max-width: 1780px;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    padding: 16px 0;
    margin: 0 auto;
  }

    &-phone {
      font-size: 22px;
      font-weight: 600;
      color: #ffffff;
      display: inline-block;
    }

    &-logo {
      color: #ffffff;
    }
}
</style>
