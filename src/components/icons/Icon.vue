<template>
  <img class="Logo__views" :src="views" alt="">
</template>

<script>
//  import { ref } from 'vue'

export default {
  name: 'LogoIcon',
  components: {
  },
  props: {
    views: {
      type: String,
      default: 'Logo'
    }
  },
  setup () {
  }
}
</script>

<style lang="scss" scoped>
.Logo__views {
  /* Logo */
  width: 120px;
  height: 34px;
  margin-left: 70px;
  margin-top: 13px;
  margin-bottom: 13px;
}
</style>
