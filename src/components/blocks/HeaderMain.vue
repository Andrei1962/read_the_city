<template>
  <header class="header">
    <div class="container">
      <img class="logo" src="@/assets/images/LocoCompany.svg" alt="">
      <a class="phone" href="">+7 987 654 32-10</a>
    </div>
  </header>
</template>

<script>

export default {
  name: 'HeaderMain',
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
}

.container {
  max-width: 1780px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin: 0 auto;
  padding: o 70px 0 70 px;
}

.phone {
  font-size: 22px;
  font-weight: 600;
  color: #ffffff;
  display: inline-block;
  text-decoration: none;
}

.logo {
  color: #ffffff;
}

</style>
