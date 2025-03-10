<template>
  <div class="list">
    <BookCard
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
import BookCard from '@/components/elements/BookCard.vue'

export default {
  name: 'ListCards',
  components: {
    BookCard
  },
  props: {
  },
  setup () {
    const dataBooks = ([
      {
        name: 'Skyrim. История сщздания великой игры',
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
  gap: 10px;
  align-items: center;
  justify-content: center;
  padding: 16px 0;
}
</style>
