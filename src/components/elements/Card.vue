<template>
<div class="card">
  <div class="card__image">
    <img class="card__preview" :src="preview" alt="">
  </div>
  <div class="card__description">
    <h2 class="card__name">
      {{ title }}
    </h2>
    <h3 class="card__author">
      {{ author }}
    </h3>
  </div>
  <!-- <span class="card__price">{{ price }}</span> -->
  <ButtonCard />
  <!-- <button class="card__button">Купить</button> -->
</div>
</template>

<script>
//  import { ref } from 'vue'
import ButtonCard from '@/components/ui/Button.vue'

export default {
  name: 'CardElement',
  components: {
    ButtonCard
  },
  props: {
    preview: {
      type: String,
      default: ''
    },
    title: {
      type: String,
      default: ''
    },
    author: {
      type: String,
      default: ''
    },
    price: {
      type: String,
      default: ''
    }
  },
  setup () {
  }
}
</script>

<style lang="scss" scoped>
.card {
  width: 330px;
  height: 490px;
  border-radius: 10px;
/* Тень серая */
  box-shadow: 1px 1px 4px 0px rgba(0, 0, 0, 0.3);
/* Белый */
  background: rgb(255, 255, 255);
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: flex-end;
}
.card__image {
  height: 270px;
  margin-top: 19px;
  // margin-bottom: 16px;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.card__preview {
  margin: 0px 0px;
  padding: 0px 0px;
  margin-left: auto;
  margin-right: auto;
  height: 100%;
}

.card__description {
 margin-top: 16px;
 height: 93px;
 display: flex;
 flex-direction: column;
 justify-content: center;
 padding: 0px;
 //margin-bottom: 20px;
}
.card__name {
  height: 56px;
  color: rgb(0, 0, 0);
  font-family: Roboto;
  font-size: 24px;
  font-weight: 400;
  line-height: auto;
  letter-spacing: 0%;
  text-align: center;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: center;
  padding: 0px;
  margin: 14px;
}

.card__author{
  color: rgb(0, 0, 0);
  font-family: Roboto;
  font-size: 20px;
  font-weight: 400;
  line-height: auto;
  letter-spacing: 0%;
  text-align: left;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: center;
  padding: 0px;
  margin: 0px;
}
</style>
