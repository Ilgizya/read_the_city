<template>
<main class="main">
  <Card
  :preview="require('@/assets/images/image_1.png')"
  title="Skyrim. История создания великой игры"
  author="Франк Экстанази"
  />
  <Card
  :preview="require('@/assets/images/image_2.png')"
  title="Поисковое продвижение сайтов"
  author="Сергей Анисимов"
  />
  <Card
  :preview="require('@/assets/images/image_3.png')"
  title="Английский для дизайнеров"
  author="Татьяна Магарина"
  />
  <Card
  :preview="require('@/assets/images/image_4.png')"
  title="Дизайн и цвет. Практикум"
  author="Шон Адамс"
  />
  </main>
</template>

<script>
//  import { ref } from 'vue'
import Card from '@/components/elements/Card'

export default {
  name: 'MainPage',
  components: {
    Card
  },
  props: {
  },
  setup () {
  }
}
</script>

<style lang="scss" scoped>
</style>
