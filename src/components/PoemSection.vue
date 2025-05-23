<template>
  <div class="poem">
    <q-parallax :height="400" :speed="0.5">
      <template v-slot:media>
        <img class="peom__img" :src="imgSrc">
      </template>
      <div class="poem__overlay"></div>

      <div class="poem__text">
        <div>
          <p v-for="(item, index) in texts" :key="index" :class="item.class">
            {{ item.text }}
          </p>
        </div>
      </div>
    </q-parallax>
  </div>
</template>

<script setup>
import { computed } from 'vue';


const props = defineProps(['image', 'texts'])

const imgSrc = computed(() => new URL(`/src/assets/img/${props.image}`, import.meta.url).href)

</script>

<style scoped lang="scss">
.poem {
  &__text {
    width: 100%;
    height: 100%;
    position: relative;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    font-size: 28px;
    color: $secondary;
    font-family: "Noto Nastaliq Urdu", serif;
    z-index: 2;
    direction: rtl;
    font-weight: bold;

    // line-height: normal;
    p {
      margin-bottom: 10px;

      &.comma {
        text-align: center;
      }
    }

    @media (max-width: 450px) {
      font-size: 22px;
      /* … */
    }

  }

  &__overlay {
    position: absolute;
    inset: 0;
    background-color: $primary;
    opacity: 0.45;
    z-index: 1;
  }

  &__img {
    opacity: 0.9;
    // width: 100%;
    // height: 100%;
  }
}
</style>
