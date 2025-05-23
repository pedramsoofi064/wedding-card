<template>
  <div class="invite-wrapper">
    <!-- Hidden SVG for clip path -->
    <div class="invite">
      <div class="overlay-text">
        <div class="names">Negin & Pedram</div>
        <div class="dates">
          <span class="date">1404.03.28</span>
          -
          <span class="date">2025.06.18</span>
        </div>
        <span class="line"></span>
        <div class="place">
           <span>TAKHTEH JAMSHID PLAZA</span>
           <span>MASHHAD</span>
        </div>

      </div>
    </div>
  </div>
</template>

<script setup>
</script>

<style lang="scss">
.invite-wrapper {}

.invite {
  // width: 320px;
  height: 90vh;
  background-size: cover;
  background-position: center;
  background-image: url('../assets/img/hero.JPG');
  position: relative;
  display: flex;
  align-items: flex-end;
  justify-content: center;
  color: white;
  padding-bottom: 50px;
  // mask-size: 100% 100px;

  .names {
    font-family: "Love Light", cursive;

    font-weight: 500;
    font-size: 70px;
    height: 75px;

    @media (max-width: 450px) {
      font-size: 22px;
      font-size: 45px;
      /* … */
    }

  }
  .dates {
    display: flex;
    gap: 10px;
    font-family: "Comme", sans-serif;
    font-size: 14px;
    font-weight: 500;
  }
  .line {
    width: 1px;
    height: 20px;
    background-color: white;
  }

  .place {
    display: flex;
    flex-direction: column;
    align-items: center;
    font-family: "Comme", sans-serif;
    font-size: 14px;
  }
}

.overlay-text {
  // text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 10px;

}
</style>
