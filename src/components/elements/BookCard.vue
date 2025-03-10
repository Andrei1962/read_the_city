<template>
  <div class="card">
    <img :src="srcImg" alt="" class="card__image">
    <h2 class="card__title">{{ title }}</h2>
    <p class="card__subtitle">{{ subtitle }}</p>
    <BaseButton name="Купить"/>
  </div>
</template>

<script>
// import { ref } from 'vue'
import BaseButton from '@/components/ui/BaseButton.vue'

export default {
  name: 'BookCard',
  components: {
    BaseButton
  },
  props: {
    title: {
      type: String,
      default: ''
    },
    subtitle: {
      type: String,
      default: ''
    },
    srcImg: {
      type: String,
      default: ''
    }
  },
  setup () {
  }
}
</script>
