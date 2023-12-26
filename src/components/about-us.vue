<script setup lang="ts">
import BouttonComponent from '@/components/boutton-component.vue'
import StraithDots from '@/components/icons/StraightDots.vue'
</script>

<template>
  <div class="container">
    <div class="left-container">
      <div class="title1">About Us</div>
      <div class="content">
        We’re a team of four passioned people.

        <p>We’re ready to take the world by storm and let you find new travel opportunities.</p>
        <p>
          Our everyday task is to make sure that you satisfied with the services and products that
          we provide.
        </p>

        With 💖 from Amsterdam, Netherlands.
      </div>
      <div>
        <BouttonComponent bouttonValue="READ MORE ABOUT US" widthSize="282px" heightSize="62px" />
      </div>
    </div>

    <div class="right-container">
      <div>
        <div class="image-item" style="background-image: url('../../src/assets/images/image1.jpeg')">
          <div class="ceo-card">MARTIN JACK, <span>CEO</span></div>
        </div>
        <div class="image-item" style="background-image: url('../../src/assets/images/image3.jpeg')"></div>
      </div>
      <div>
        <div class="image-item" style="background-image: url('../../src/assets/images/image2.jpeg')"></div>
        <div class="image-item" style="background-image: url('../../src/assets/images/image4.jpeg')"></div>
        <div class="dots-container">
          <div v-for="index in 4" :key="index">
            <StraithDots />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.container {
  top: 0;
  left: 0;
  width: 100%;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 100px;
}

.image-item {
  width: 50%;
  height: 395px;
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
}

.left-container {
  width: 340px;
  height: 100%;
  display: flex;

  flex-direction: column;
  align-items: start;
  justify-content: center;
  margin-top: -180px;
  gap: 22px;
}
.right-container {
  width: 800px;

  display: flex;
  flex-direction: row;
  position: relative;
}

.right-container > div,
.image-item {
  width: 100%;
  position: relative;
}

.right-container > div:nth-child(2) {
  position: relative;

  z-index: 9;
}
.dots-container {
  position: absolute;
  top: 25%;
  right: -100px;

  z-index: 999;
  width: 100px;
  height: 60%;
}

.title1 {
  color: #fff;
  text-align: center;
  font-family: 'Noe Display', serif;
  font-size: 72px;
  font-style: normal;
  font-weight: 700;
  line-height: 110%; /* 79.2px */
  letter-spacing: -1.44px;
}

.content {
  color: #fff;

  font-family: 'Larsseit', sans-serif;
  font-size: 18px;
  font-style: normal;
  font-weight: 800;
  line-height: 150%; /* 27px */
  letter-spacing: -0.36px;

  display: flex;
  flex-direction: column;
  gap: 20px;
  margin-bottom: 38px;
}

p {
  color: #fffc;
  font-family: 'Larsseit', sans-serif;
  font-size: 18px;
  font-style: normal;
  font-weight: 300;
  line-height: 150%;
  letter-spacing: -0.36px;
}

.ceo-card {
  width: 186px;
  height: 75px;
  flex-shrink: 0;
  border-radius: 8px;
  background: #fff;

  /* Button Shadow */
  box-shadow: 5px 15px 40px 0px rgba(0, 201, 224, 0.2);
  color: #000;
  font-family: 'Larsseit', sans-serif;
  font-size: 15px;
  font-style: normal;
  font-weight: 700;
  line-height: 150%; /* 22.5px */
  letter-spacing: 0.75px;

  display: flex;
  justify-content: center;
  align-items: center;
  position: absolute;
  bottom: 0;
  left: -20%;
  margin-bottom: 20%;
}

.ceo-card > span {
  color: #00c9e0;
  font-family: 'Larsseit', sans-serif;
  font-size: 15px;
  font-style: normal;
  font-weight: 700;
  line-height: 150%;
  letter-spacing: 0.75px;
}
</style>
