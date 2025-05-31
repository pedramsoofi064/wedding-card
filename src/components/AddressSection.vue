<template>
  <div class="address">
    <div class="address__boxes">
      <div class="address__item">
        <span class="item__title">آدرس تالار</span>
        <span class="item__value"> ابتدای شاندیز ، خیابان امام رضا(ع)، بعد از امام رضا 3</span>
      </div>
      <div class="address__item">
        <span class="item__title">مسیریابی </span>
        <div class="link-container">
          <a class="link-item" href="https://maps.app.goo.gl/5QEjcMBsp7u6bRTBA" target="_blank">
            <img src="../assets/img/google-maps.webp" />
          </a>
          <a class="link-item" href="https://nshn.ir/08_b10EDNJWb2r" target="_blank">
            <img src="../assets/img/neshan.webp" />
          </a>
        </div>
      </div>
    </div>

  </div>
  <div class="address__location">
    <iframe
      src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d1605.4312579909426!2d59.35014260000001!3d36.41252149999998!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3f6cf6441f369d45%3A0x2b41631e08005afb!2sTakhte%20Jamshid%20Restaurant!5e0!3m2!1sen!2s!4v1748003968149!5m2!1sen!2s"
      width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy"
      referrerpolicy="no-referrer-when-downgrade"></iframe>
  </div>
</template>

<script setup>

</script>


<style lang="scss" scoped>
.address {
  // padding: 50px;
  // padding-bottom: 0;
  direction: rtl;
  font-family: "Peyda";
  margin-block: 1rem;
  padding-inline:2rem;

  &__boxes {
    display: grid;
    grid-template-columns: 1fr ;
    gap: 10px;
    font-family: "Vazirmatn", sans-serif;

  }

  &__item {
    // padding: 20px;
    padding: 5px;
    border-radius: 10px;
    background-color: #f1e9de;
    display: flex;
    flex-direction: column;
    align-items: center;
    color: #585045;

    .item__title {
      font-size: 24px;
      font-weight: bold;
    }

    .item__value {
      margin-top: 5px;
    }

    .link-container {
      display: flex;
      gap: 15px;
      margin-top: 5px;

      .link-item {
        >img {
          width: 35px;
        }
      }
    }
  }

  &__location {
    width: 100%;

    >iframe {
      width: 100%;
    }
  }
}
</style>
