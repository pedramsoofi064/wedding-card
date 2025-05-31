<template>
  <div class="invite-wrapper">
    <!-- Hidden SVG for clip path -->
    <div class="invite-mobile">
      <div class="img-bg">
      </div>
      <div class="info">
        <div class="names negin">Negin</div>
        <div class="names pedram">Pedram</div>
        <div class="dates">
          <span class="date">1404.03.28</span>
          -
          <span class="date">2025.06.18</span>
        </div>
        <!-- <span class="line"></span>
        <div class="place">
           <span>TAKHTEH JAMSHID PLAZA</span>
           <span>MASHHAD</span>
        </div> -->

      </div>
    </div>

    <div class="wedding-text">The wedding time</div>
  </div>
</template>

<script setup>
</script>

<style lang="scss">
.invite-wrapper {}

.invite-mobile {
  // width: 320px;
  // height: 100vh;
  position: relative;
  min-height: 110vh;
  display: flex;


  .img-bg {
    position: absolute;
    inset: 0;
    height: 110vh;
    background-image: url(../assets/img/hero.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    filter: blur(2px);


    // >img {
    //   width: 100%;
    //   height: 100%;
    //   z-index: 1;
    // }
  }




  .info {
    position: absolute;
    bottom: 45%;
    color: white;
    display: flex;
    flex-direction: column;
    z-index: 6;
    margin-left: 20px;
    width: 100%;
  }

  .names {
    font-family: "Love Light", cursive;

    font-weight: 500;
    font-size: 110px;
    height: 140px;
    &.pedram  {
      margin-left: 20%;
    }

  }

  .dates {
    display: flex;
    gap: 10px;
    font-family: "Comme", sans-serif;
    font-size: 14px;
    font-weight: 500;
    margin-inline: auto;
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



.wedding-text {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 50px;
  font-family: "Love Light", cursive;
  color: #b0a08a;
  position: relative;

  &::before {
    content: "";
    background-image: url('../assets/img/torn1.png');
    position: absolute;
    background-size: cover;
    bottom: 97%;
    height: 65px;
    width: 100%;
    left: 0;
    background-repeat: no-repeat;
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
