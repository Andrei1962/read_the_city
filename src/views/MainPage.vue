<template>
  <div class="home">
    <TheHeader/>
    <ListCards/>
  </div>
</template>

<script>
// @ is an alias to /src
import TheHeader from '@/components/blocks/TheHeader.vue'
import ListCards from '@/components/blocks/ListCards.vue'

export default {
  name: 'HomeView',
  components: {
    TheHeader,
    ListCards
  },
  setup () {
  }
}
</script>
<style lang="scss" scoped>
</style>
