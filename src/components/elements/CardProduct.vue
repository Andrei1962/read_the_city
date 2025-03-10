<template>
  <div class="card">
    <img :src="srcImg" alt="" class="image">
    <h2 class="title">{{ title }}</h2>
    <p class="subtitle">{{ subtitle }}</p>
    <ButtonCard class="button" name="Купить"/>
  </div>
</template>

<script>
// import { ref } from 'vue'
import ButtonCard from '@/components/ui/ButtonCard.vue'

export default {
  name: 'CardProduct',
  components: {
    ButtonCard
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

<style>
.card {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  text-align: center;
  gap: 10px;
  width: 330px;
  height: 490px;
  border-radius: 10px;
  border: 1px solid rgb(141, 79, 79);
}

.image {
  padding-top: 19px;
}

.title {
  font-family: "Roboto" , sans-serif;
  font-size: 24px;
  font-weight: 400;
  line-height: 28px;
  color: #000;
  margin: 0 14px 0 14px;
}

.subtitle {
  font-size: 20px;
  font-weight: 400;
  line-height: 23px;
}

.button {
  background-color: #3278ff;
  color: #ffffff;
  padding: 6px 38px;
  border-radius: 7px;
  font-size: 20px;
  font-weight: 400;
  margin-bottom: 24px;
}
</style>
