<template>
<header class="header">
  <IconLogo
  :views="require('@/assets/Logo_1.png')"
  />
  <p class="header__phone">
    +7 987 654 32-10
  </p>
</header>
</template>

<script>
//  import { ref } from 'vue'
import IconLogo from '@/components/icons/Icon.vue'

export default {
  name: 'HeaderPage',
  components: {
    IconLogo
  },
  props: {
  },
  setup () {
  }
}
</script>

<style lang="scss" scoped>
.header {
  display: flex;
  margin-top: 0px;
  background: rgb(50, 120, 255);
  width: 1920px;
  height: 60px;
  margin-bottom: 235px;
  flex-direction: row;
}
.header__phone {
  width: 175px;
  height: 26px;
  margin-left: 1430px;
  margin-top: 16px;
  margin-bottom: 18px;
  color: rgb(255, 255, 255);
  font-family: Roboto;
  font-size: 22px;
  font-weight: 600;
  line-height: 26px;
  letter-spacing: 0%;
  text-align: left;
}
</style>
