<template>
  <q-page>
    <!-- <div class="q-pa-none scroll-container">
      <MainHero class="page" />
      <BannerSection class="page" />
      <div class="page">
        <TimeLineSection />

      </div>
    </div> -->
    <div class="fullpage">
      <div class="fullpage-bg"></div>
      <div class="page-container">

        <MainHero />
        <!-- <div class="wedding-time">
        the wedding time
      </div> -->
        <InvitationText />
        <PoemSection image="test3-1.jpg" :texts="peom" />
        <TimeLineSection />
        <CountDownSection />
        <AddressSection />
      </div>
    </div>






  </q-page>
</template>

<script setup>
import MainHero from 'src/components/MainHero.vue';
// import BannerSection from 'src/components/BannerSection.vue';
import TimeLineSection from 'src/components/TimeLineSection.vue';
import PoemSection from 'src/components/PoemSection.vue';
import CountDownSection from 'src/components/CountDownSection.vue';
import InvitationText from 'src/components/Invitation-text.vue';
import AddressSection from 'src/components/AddressSection.vue';


const peom = [
  { class: 'line', text: 'اشتیاقی که به دیدار تو‌ دارد دل من،' },
  { class: 'line', text: 'دل من داند و‌ من دانم و دل داند و من .' },
  { class: 'comma', text: '،،،' },
  { class: 'line', text: 'خاک من گل شود و گل شکفد از گل من،' },
  { class: 'line', text: 'تا ابد مهر تو بیرون نرود از دل من.' }
];
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

.wedding-time {
  width: 100%;
  height: 10vh;
  background-color: #f1e9de;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 50px;
  font-family: "Love Light", cursive;
  color: #585045;
}

.fullpage {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;

}

.fullpage-bg {
  background-image: url('../assets/img/bg.jpg');
  background-size: cover;
  /* background-position: center; */
  filter: blur(5px);
  position: fixed;
  z-index: -1;
  inset: 0;
}

.page-container {
  max-width: 480px;
  box-shadow: rgba(0, 0, 0, 0.1) 0px 4px 12px;
  background-color: white;

}
</style>
