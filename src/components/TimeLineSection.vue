<template>
  <div class="q-px-lg q-py-md">

    <div class="texts">
    </div>
    <q-timeline layout="loose" color="primary">

      <q-timeline-entry side="left">
        <template #title>
          <div class="timeline-item">
            <locationIcon class="timeline-item__icon" />

            <div class="timeline-item__time">18:00</div>
            <div class="timeline-item__title">Welcome</div>
          </div>
        </template>
      </q-timeline-entry>

      <q-timeline-entry side="right">
        <template #title>
          <div class="timeline-item">
            <locationIcon class="timeline-item__icon" />

            <div class="timeline-item__time">18:00</div>
            <div class="timeline-item__title">Welcome</div>
          </div>
        </template>

      </q-timeline-entry>

      <q-timeline-entry side="left">
        <template #title>
          <div class="timeline-item">
            <locationIcon class="timeline-item__icon" />

            <div class="timeline-item__time">18:00</div>
            <div class="timeline-item__title">Welcome</div>
          </div>
        </template>

      </q-timeline-entry>
    </q-timeline>
  </div>
</template>

<script setup>

import locationIcon from './icons/location-icon.vue'

</script>

<style scoped lang="scss">
.texts {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-block: 30px;
  font-family: "Vazirmatn", sans-serif;
  font-optical-sizing: auto;
  font-size: 30px;
  color: $primary;

  >p {
    font-weight: 500;
    text-align: center;
  }
}

.timeline-item {
  display: flex;
  flex-direction: column;
  // align-items: flex-end;
  align-items: center;
  justify-content: center;
  color: $primary;
  gap: 0.5rem;

  &__icon {
    width: 100px;
    fill: $primary;
  }

  &__time {
    font-size: 20px;
    font-weight: bold;
  }

  &__title {}
}
</style>
