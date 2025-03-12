<template>
  <div class="list">
    <CardProduct
      v-for="(item, i) in dataBooks"
      :key="i"
      :title="item.name"
      :subtitle="item.description"
      :srcImg="item.image"
    />
  </div>
</template>

<script>
// import { ref } from 'vue'
import CardProduct from '@/components/elements/CardProduct.vue'

export default {
  name: 'MainCards',
  components: {
    CardProduct
  },
  props: {
  },
  setup () {
    const dataBooks = ([
      {
        name: 'Skyrim. История создания великой игры',
        description: 'Франк Экстанази',
        image: require('@/assets/images/book_1.png')
      },
      {
        name: 'Поисковое продвижение сайтов',
        description: 'Сергей Анисимов',
        image: require('@/assets/images/book_2.png')
      },
      {
        name: 'Английский для дизайнеров',
        description: 'Татьяна Магарина',
        image: require('@/assets/images/book_3.png')
      },
      {
        name: 'Дизайн и цвет. Практикум',
        description: 'Шон Адамс',
        image: require('@/assets/images/book_4.png')
      }
    ])

    return {
      dataBooks
    }
  }
}
</script>

<style lang="scss" scoped>

.list {
  display: flex;
  gap: 26px;
  align-items: center;
  justify-content: center;
  height: calc(100vh - 60px);
}
</style>
