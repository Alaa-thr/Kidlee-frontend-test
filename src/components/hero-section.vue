<script setup lang="ts">
import IconSearch from '@/components/icons/IconSearch.vue'
import SocialMedia from '@/components/icons/SocialMedia.vue'
import ButtonComponent from '@/components/boutton-component.vue'
</script>

<template>
  <div class="container">
    <header>
      <div>
        <IconSearch class="btn" />
        <ButtonComponent bouttonValue="Menu" widthSize="200px" heightSize="62px" />
      </div>
      <div>NT<span style="color: #41ead4">.</span></div>
    </header>

    <div class="body">
      <div>
        <div class="body-title m-b-14">Night Trips</div>
        <div class="body-subtitle m-b-50">WE GOT TRIPS FOR THE TRIPPSTER IN YOU</div>
        <p class="body-content">
          Neque, eros commodo, nascetur ullamcorper vitae. Tincidunt ut venenatis, volutpat lorem ut
          faucibus mauris, quisque. Integer gravida sed quis congue. Vel risus, arcu a viverra leo
          id pulvinar ultricies. Enim in in in pulvinar nulla sollicitudin. Ullamcorper.
        </p>
      </div>
    </div>

    <div class="footer">
      <div id="footer-scroll-text">
        <div class="line"></div>
        <div>SCROLL</div>
      </div>
      <div class="social-media-container">
        <SocialMedia type="Twitter" />
        <SocialMedia type="Instagram" />
        <SocialMedia type="Facebook" />
      </div>
    </div>
  </div>
</template>

<style scoped>
.container {
  top: 0;
  left: 0;
  width: 100%;
  height: 1000px;
  background-image: url('../assets/images/hero-section.jpeg');
  background-repeat: no-repeat;
  background-size: 120%; 
  background-position:  right center;
}

header {
  display: flex;
  flex-direction: column;
  padding: 31px 263px;
}

header > div:first-child {
  display: flex;
  flex: 1;
  justify-content: flex-end;
  align-items: center;
  gap: 37px;
}

header > div:nth-child(2) {
  color: #fff;
  font-family: 'Playfair Display', serif;
  font-size: 36px;
  font-style: normal;
  font-weight: 700;
  line-height: 190%; /* 68.4px */
}
.body {
  padding: 80px 263px;
  margin-left: 150px;
}
.body > div:first-child {
  width: 590px;
  margin-bottom: 106px;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.body-title {
  color: #fff;
  font-family: 'Noe Display', serif;
  font-size: 120px;
  font-style: normal;
  font-weight: 700;
  line-height: normal;
  letter-spacing: -2.4px;
}
.body-subtitle {
  color: #fff;
  font-family: 'Larsseit', sans-serif;
  font-size: 18px;
  font-style: normal;
  font-weight: 700;
  line-height: normal;
  letter-spacing: 1.8px;
  text-transform: uppercase;
}
.body-content {
  color: #fff;
  text-align: center;
  font-family: 'Larsseit', sans-serif;
  font-size: 17px;
  font-style: normal;
  font-weight: 400;
  line-height: 150%;
  width: 650px;
}
.footer {
  display: flex;
  justify-content: space-between;
  height: 30%;
  flex-shrink: 0;
  background: linear-gradient(180deg, rgba(1, 22, 39, 0) 0%, #011627 76.64%, #011627 100%);
  padding: 50px 220px;

}

#footer-scroll-text {
  margin-left: -50px;
  margin-top: 60px;
  display: flex;
  align-items: center;
  gap: 15px;
  height: fit-content;
  transform: rotate(-90deg);
}

#footer-scroll-text > div:first-child {
  width: 80px;
  height: 2px;
  flex-shrink: 0;
  border-radius: 13px;
  background: linear-gradient(180deg, #09f4f4 0%, #00c9e0 100%);
}
#footer-scroll-text > div:nth-child(2) {
  color: #fff;
  font-family: 'Larsseit', sans-serif;
  font-size: 15px;
  font-style: normal;
  font-weight: 700;
  line-height: 190%; /* 28.5px */
  letter-spacing: 0.75px;
}

.social-media-container {
  height: fit-content;
  display: flex;
  flex-direction: column;
  gap: 20px;
}

</style>
