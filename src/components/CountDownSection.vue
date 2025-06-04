<template>
  <div class="countdown">
    <div class="timer">
      <div class="time-unit">
        <span class="number">{{ countdown.days }}</span>
        <span class="label">روز</span>
      </div>
      <div class="time-unit">
        <span class="number">{{ countdown.hours }}</span>
        <span class="label">ساعت</span>
      </div>
      <div class="time-unit">
        <span class="number">{{ countdown.minutes }}</span>
        <span class="label">دقیقه</span>
      </div>
      <div class="time-unit">
        <span class="number">{{ countdown.seconds }}</span>
        <span class="label">ثانیه</span>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from 'vue'

const countdown = ref({
  days: 0,
  hours: 0,
  minutes: 0,
  seconds: 0
})

// 🎯 Set your wedding date here
const targetDate = new Date('2025-06-17T18:00:00+03:30')

const updateCountdown = () => {
  const now = new Date()
  const diff = targetDate - now

  if (diff <= 0) {
    countdown.value = { days: 0, hours: 0, minutes: 0, seconds: 0 }
    return
  }

  const totalSeconds = Math.floor(diff / 1000)
  countdown.value.days = Math.floor(totalSeconds / (60 * 60 * 24))
  countdown.value.hours = Math.floor((totalSeconds / 3600) % 24)
  countdown.value.minutes = Math.floor((totalSeconds / 60) % 60)
  countdown.value.seconds = totalSeconds % 60
}

let interval
onMounted(() => {
  updateCountdown()
  interval = setInterval(updateCountdown, 1000)
})

onUnmounted(() => {
  clearInterval(interval)
})
</script>

<style scoped>
.countdown {
  text-align: center;
  padding: 1rem;
  padding-top: 25px;
  background-color: #f1e9de;
  color: #585045;
  font-family: "Peyda", sans-serif;
}

.title {
  font-size: 2rem;
  font-weight: bold;
  margin-bottom: 2rem;
}

.timer {
  display: flex;
  justify-content: center;
  gap: 2rem;
  flex-wrap: wrap;
}

.time-unit {
  display: flex;
  flex-direction: column;
  align-items: center;
  font-weight: bold;
  font-size: 20px;
}

.number {
  font-size: 3rem;
}

.label {
 
}
</style>
