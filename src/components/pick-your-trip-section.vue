<script setup lang="ts">
import Dots from '@/components/icons/Dots.vue'
import SliderController from '@/components/icons/SliderController.vue'
import ButtonComponent from '@/components/boutton-component.vue'
import SocialMedia from '@/components/icons/SocialMedia.vue'
</script>

<template>
  <div class="container">
    <div class="header">
      <span class="title">Pick your trip</span>
      <div>
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="24"
          height="24"
          viewBox="0 0 24 24"
          fill="none"
        >
          <path
            d="M18 6L6 18"
            stroke="#41EAD4"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
          <path
            d="M6 6L18 18"
            stroke="#41EAD4"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
        </svg>
      </div>

      <div class="title2">
        Our team put together some trips to you to discover, feel free to discover each of them.
      </div>
    </div>
    <div class="body">
      <div class="nav">
        <div class="nav-item active btn">
          <div class="title-nav-item">Chill Adventure</div>
          <div class="line"></div>
        </div>
        <div class="nav-item disabled btn">
          <div class="title-nav-item">Spooky Times</div>
          <div class="line"></div>
        </div>
        <div class="nav-item disabled btn">
          <div class="title-nav-item">Desert Madness</div>
          <div class="line"></div>
        </div>
        <div class="nav-item disabled btn">
          <div class="title-nav-item">Out in the wild</div>
          <div class="line"></div>
        </div>
      </div>
      <div class="nav-line"></div>
      <div class="box">
        <div class="image-box">
          <div class="gimmick-line">
            <svg xmlns="http://www.w3.org/2000/svg" width="172" height="13" viewBox="0 0 172 13" fill="none">
              <rect width="172" height="2" rx="1" fill="#41EAD4"/>
              <path d="M0 1H2V12C2 12.5523 1.55228 13 1 13C0.447715 13 0 12.5523 0 12V1Z" fill="#41EAD4"/>
            </svg>
          </div>
          <div>01.</div>
          <div >GRAND DUNES LANDSCAPE</div>
          <div>
            <Dots class="dots"/>
            <div class="slider-controller">
              <SliderController type="Left"/>
              <div class="slider-bar"></div>
              <SliderController type="Right"/>
            </div>
          </div>
        </div>
        <div class="text-box">
          <div>Chill Adventure</div>
          <p class="paragraph1 m-t-32">
            Ornare vivamus molestie pellentesque nunc. Sed sapien erat ultrices curabitur. 
            Erat id fringilla arcu condimentum fames.
          </p>
          <p class="paragraph2 m-t-32 m-b-45"> Aliquet dictum aliquet faucibus cursus turpis. Suspendisse cum rutrum sit ut sociis. 
            Pellentesque neque orci adipiscing pharetra lacus, dignissim pharetra ipsum blandit. 
            Feugiat quis quam consectetur lectus id quis tortor vel, mattis.
          </p>
          <ButtonComponent bouttonValue="SEE OUR LATEST OFFER" widthSize="282px" heightSize="65px"/>
         
        </div>
        <div class="social-media-box">
          <div class="share-it-text">SHARE IT:</div>
          <div class="social-media-container">
            <SocialMedia type="Instagram" />
            <SocialMedia type="Facebook" />
            <SocialMedia type="Twitter" />
          </div>
          <div>
            <svg xmlns="http://www.w3.org/2000/svg" width="133" height="32" viewBox="0 0 133 32" fill="none">
              <rect x="133" y="32" width="133" height="2" rx="1" transform="rotate(180 133 32)" fill="#41EAD4"/>
              <path d="M133 31H131V1C131 0.447718 131.448 0 132 0C132.552 0 133 0.447716 133 1V31Z" fill="#41EAD4"/>
            </svg>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.container {
  margin: 58px 266px 232px 299px;
}
.box{
  display: flex;
  height: 10%;
  margin-left: 95px;
}
.image-box{
  border-radius: 8px;
  background: url('../assets/images/dessert-image.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  width: 486px;
  height: 607px;
  flex-shrink: 0;
  margin-right: 126px;
}
.nav-line{
  width: 1200px;
  height: 2px;
  flex-shrink: 0;
  border-radius: 13px;
  opacity: 0.3;
  background: #41EAD4;
  margin-bottom: 150px;
  margin-left: 95px;
  margin-top: -2px;
}
.slider-bar{
  width: 2px;
  height: 65px;
  flex-shrink: 0;
  opacity: 0.5;
  background: #133149;
}
.image-box > div:nth-child(2){
  color: #41EAD4;
  font-family: 'Larsseit',sans-serif;
  font-size: 24px;
  font-style: normal;
  font-weight: 800;
  line-height: 150%; /* 36px */
  letter-spacing: 3.6px;
  margin-left: -95px;
}
.image-box > div:nth-child(3){
  color: #FFF;
  font-family: 'Larsseit',sans-serif;
  font-size: 24px;
  font-style: normal;
  font-weight: 700;
  line-height: 150%; /* 36px */
  letter-spacing: 3.6px;
  margin-left: -95px;
  margin-bottom: 82px;
  width: 220px;
  flex-shrink: 0;
}
.image-box > div:nth-child(4){
  display: flex;
  margin-left: -55px;
}
.slider-controller{
  display:flex;
  align-items: center;
  justify-content: end; 
  width: 100%;
}
.dots{
  width: 230px;
  height: 230px;
  flex-shrink: 0;
}
.gimmick-line{
  margin-top: 254px; 
  margin-left: -95px;
}
.text-box{
  width: 62%;
  margin-top: 88px;
}
.text-box > div:first-child{ 
  color: #FFF;
  font-family: Noe Display;
  font-size: 65px;
  font-style: normal;
  font-weight: 700;
  line-height: 110%; /* 71.5px */
  letter-spacing: -1.3px;
}
.paragraph1{
  color: #FFF;
  font-family: 'Larsseit', sans-serif;
  font-size: 17px;
  font-style: normal;
  font-weight: 700;
  line-height: 150%; /* 25.5px */
  letter-spacing: -0.34px;
}
.paragraph2{
  color: #FFF;
  font-family: 'Larsseit', sans-serif;
  font-size: 17px;
  font-style: normal;
  font-weight: 400;
  line-height: 150%;
  letter-spacing: -0.34px;
}
.header {
  display: flex;
  flex-direction: row;
  align-items: center;
  gap: 33px;
  margin-left: 93px;
  margin-bottom: 83px;
}
.title {
  color: #fff;
  text-align: center;
  font-family: 'Noe Display', serif;
  font-size: 72px;
  font-style: normal;
  font-weight: 700;
  line-height: 110%; /* 79.2px */
  letter-spacing: -1.44px;
}
.title2 {
  color: #fff;
  font-family: 'Larsseit', sans-serif;
  font-size: 15px;
  font-style: normal;
  font-weight: 400;
  line-height: 150%; /* 24px */
  letter-spacing: -0.32px;
  width: 350px;
}
.share-it-text{
  color: #FFF;
  font-family: 'Larsseit', sans-serif;
  font-size: 16px;
  font-style: normal;
  font-weight: 700;
  line-height: 150%; /* 22.5px */
  letter-spacing: 2.25px;
}
.title-nav-item{
  text-align: center;
  font-family: 'Larsseit', sans-serif;
  font-size: 15px;
  font-style: normal;
  font-weight: 700;
  line-height: 110%; /* 19.8px */
  letter-spacing: -0.36px;
}
.nav{
  display: flex;
  flex-shrink: 0;
  margin-left: 95px;
}
.nav-item{
  width: 24%;
  height: 57px;
  flex-shrink: 0;
}
.nav-item > div:first-child{
  padding-bottom: 33px;
}
.nav-item.active > div:nth-child(2){
  width: 100%;
  height: 4px;
  flex-shrink: 0;
  border-radius: 13px;
  background: #41EAD4;
}
.nav-item.active > div:first-child{
  font-size: 18px;
  letter-spacing: -0.36px;
}
.social-media-container {
  width: fit-content;
  display: flex;
  gap: 23px;
  margin-bottom: -20px;
  margin-top: 18px;
}
.social-media-box{
  display:flex;
  align-items: start;
  justify-content: flex-end;
  flex-direction: column;
}
</style>
