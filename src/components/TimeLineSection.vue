<template>
  <div class="q-px-lg q-py-md">


    <q-timeline layout="loose" color="primary">

      <q-timeline-entry side="right">
        <template #title>
          <div class="timeline-item">
            <img class="timeline-item__icon" src="../assets/img/welcome.png" alt="">

            <div class="timeline-item__time">18:00</div>
            <div class="timeline-item__title">ورود</div>
          </div>
        </template>
      </q-timeline-entry>

      <q-timeline-entry side="left">
        <template #title>
          <div class="timeline-item">
            <img class="timeline-item__icon" src="../assets/img/wedding-rings.png" alt="">
            <div class="timeline-item__time">18:30</div>
            <div class="timeline-item__title">عقد آریایی</div>
          </div>
        </template>

      </q-timeline-entry>

      <q-timeline-entry side="right">
        <template #title>
          <div class="timeline-item">
            <img class="timeline-item__icon" src="../assets/img/camera.png" alt="">

            <div class="timeline-item__time">19:00</div>
            <div class="timeline-item__title">عکس برداری</div>
          </div>
        </template>

      </q-timeline-entry>
      <q-timeline-entry side="left">
        <template #title>
          <div class="timeline-item">
            <img class="timeline-item__icon" src="../assets/img/music.png" alt="">

            <div class="timeline-item__time">20:00</div>
            <div class="timeline-item__title">رقص</div>
          </div>
        </template>

      </q-timeline-entry>
      <q-timeline-entry side="right">
        <template #title>
          <div class="timeline-item">
            <img class="timeline-item__icon" src="../assets/img/cake.png" alt="">

            <div class="timeline-item__time">21:00</div>
            <div class="timeline-item__title">رقص چاقو</div>
          </div>
        </template>

      </q-timeline-entry>
      <q-timeline-entry side="left">
        <template #title>
          <div class="timeline-item">
            <img class="timeline-item__icon" src="../assets/img/dinner.png" alt="">

            <div class="timeline-item__time">22:00</div>
            <div class="timeline-item__title">شام</div>
          </div>
        </template>

      </q-timeline-entry>

       <q-timeline-entry side="right">
        <template #title>
          <div class="timeline-item">
            <img class="timeline-item__icon" src="../assets/img/exit.png" alt="">

            <div class="timeline-item__time">23:00</div>
            <div class="timeline-item__title">خروج</div>
          </div>
        </template>

      </q-timeline-entry>

    </q-timeline>
  </div>
</template>

<script setup>


</script>

<style scoped lang="scss">
.texts {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-block: 30px;
  font-family: "Peyda";
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
  font-family: "Peyda";

  align-items: center;
  justify-content: center;
  color: $primary;
  gap: 0.5rem;

  &__icon {
    width: 80px;
    fill: $primary;
  }

  &__time {
    font-size: 20px;
    font-weight: bold;
  }

  &__title {}
}
</style>
