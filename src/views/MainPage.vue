<template>
  <div class="home">
    <HeaderMain/>
    <MainCards/>
  </div>
</template>

<script>
// @ is an alias to /src
import HeaderMain from '@/components/blocks/HeaderMain.vue'
import MainCards from '@/components/blocks/MainCards.vue'

export default {
  name: 'HomeView',
  components: {
    HeaderMain,
    MainCards
  },
  setup () {
  }
}
</script>
<style lang="scss" scoped>
</style>
