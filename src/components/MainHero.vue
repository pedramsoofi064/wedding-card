<template>
  <div class="invite-wrapper">
    <!-- Hidden SVG for clip path -->
    <div class="invite-mobile">
      <img src="src/assets/img/test1.png" alt="">
      <div class="info">
        <div class="names">Negin & Pedram</div>
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
    <div class="invite-desktop">
      <img src="src/assets/img/org.png" alt="">
      <div class="info">
        <div class="names">Negin & Pedram</div>
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
  display: none;
  position: relative;
  max-height: 90vh;


  // @media (max-width: 400px) {
  //   min-height: 70vh;
  // }

  // @media (max-width: 450px) {
  //   display: flex;
  //   min-height: 80vh;

  // }



  @media (max-width: 520px) {
    display: flex;
    align-items: center;
    justify-content: center;
    // min-height: 80vh;

  }

  >img {
    width: 100%;
    height: 100%;
    z-index: 1;
  }



  .info {
    position: absolute;
    bottom: 30%;
    color: white;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    z-index: 6;
  }

  .names {
    font-family: "Love Light", cursive;

    font-weight: 500;
    font-size: 70px;
    height: 75px;

    @media (max-width: 500px) {
      margin-bottom: 5px;
      font-size: 60px;
    }
    @media (max-width: 450px) {
      margin-bottom: 5px;
      font-size: 50px;
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

.invite-desktop {
  // width: 320px;

  // min-height: 40vh;
  // max-height: 90vh;
  margin-bottom: 20px;
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;

  >img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    max-height: 90vh;
  }

  @media (max-width: 996px) {
    background-size: contain;
  }
  @media (max-width: 520px) {
    display: none;
  }



  .info {
    position: absolute;
    bottom: 20%;
    color: white;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    z-index: 6;
  }

  .names {
    font-family: "Love Light", cursive;

    font-weight: 500;
    font-size: 100px;
    height: 75px;

    @media (max-width: 700px) {
      font-size: 70px;

    }



  }

  .dates {
    display: flex;
    gap: 10px;
    font-family: "Comme", sans-serif;
    font-size: 25px;
    font-weight: 500;
    margin-top: 50px;


    @media (max-width: 700px) {
      font-size: 18px;

    }

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

}


.overlay-text {
  // text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 10px;

}
</style>
