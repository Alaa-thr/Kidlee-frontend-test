<script setup lang="ts">
import { defineProps, ref } from 'vue'

const props = defineProps({
  bouttonValue: {
    bouttonValue: String,
    required: true
  },
  widthSize: {
    widthSize: String,
    required: true
  },
  heightSize:{
    heightSize: String,
    required: true
  },
});
const widthSize= ref(props.widthSize);
const heightSize= ref(props.heightSize);
</script>

<template>
    <div class="btn-container">
        <div class="menu-btn btn">{{bouttonValue}}</div>
        <div class="btn-line"></div>
    </div>
</template>

<style scoped>
.btn-container{
  display: flex;
}
.menu-btn {
    width: v-bind(widthSize);
    height: v-bind(heightSize);
    border-radius: 183px;
    background: #00c9e0;
    color: #fff;
    font-family: 'Helvetica Neue', 'Helvetica', 'Arial', sans-serif;
    font-size: 16px;
    font-style: normal;
    font-weight: 700;
    line-height: normal;
    letter-spacing: 1.6px;
    text-transform: uppercase;
    box-shadow: 5px 15px 40px 0px rgba(0, 201, 224, 0.2);
    display: flex;
    justify-content: center;
    align-items: center;
}
.btn-line{
  width: 30px;
  height: 2px;
  margin-left: -15px;
  flex-shrink: 0;
  border-radius: 16px;
  background: #FFF;
  align-self: center;
}
</style>
  

  