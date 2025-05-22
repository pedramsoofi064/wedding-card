<template>
  <q-page>
    <!-- <div class="q-pa-none scroll-container">
      <MainHero class="page" />
      <BannerSection class="page" />
      <div class="page">
        <TimeLineSection />

      </div>
    </div> -->
    <MainHero />
    <TimeLineSection />

  </q-page>
</template>

<script setup>
import MainHero from 'src/components/MainHero.vue';
// import BannerSection from 'src/components/BannerSection.vue';
import TimeLineSection from 'src/components/TimeLineSection.vue';
//
</script>

<style>
.scroll-container {
  height: 100vh;
  overflow-y: scroll;
  scroll-snap-type: y mandatory;
}

.page {
  min-height: 100vh;
  scroll-snap-align: start;

}
</style>
