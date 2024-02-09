<template>
  <div class="">
    <Header />
    <Main />
</div>
</template>

<script>
//  import { ref } from 'vue'
//  import Button from '@/components/ui/Button'
import Header from '@/components/blocks/Header'
import Main from '@/components/blocks/Main'

export default {
  name: 'MainPage',
  components: {
    Header,
    Main
    //  Button
  },
  props: {
  },
  setup () {
  }
}
</script>

<style lang="scss" scoped>
.main {
  display: flex;
  justify-content: center;
  gap: 26px;
  bottom: 1020px;
  width: 1920px;
}
</style>
