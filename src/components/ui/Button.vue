<template>
<button
  :class="{
  'button': true
  }
  ">
  {{ name }}
</button>
</template>

<script>
//  import { ref } from 'vue'

export default {
  name: 'ButtonUi',
  components: {
  },
  props: {
    name: {
      type: String,
      default: 'Купить'
    }
  },
  setup () {
  }
}
</script>

<style lang="scss" scoped>
.button {
  color: white;
  background-color: blue;
  font-size: 18px;
  width: 141px;
  height: 34px;
  border-radius: 7px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 6px 38px 6px 38px;
  margin-bottom: 24px;
  margin-top: 24px;
}
</style>
