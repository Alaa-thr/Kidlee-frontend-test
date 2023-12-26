<script setup lang="ts">
import { defineProps } from 'vue'

const props = defineProps({
  type: {
    type: String as () => 'Left' | 'Right',
    required: true
  }
})
</script>

<template>
   <div v-if="type === 'Left'" class="slider-controller-left btn">
      <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
        <path d="M19 12L5 12" stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
        <path d="M12 19L5 12L12 5" stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
      </svg>
    </div>
    <div v-if="type === 'Right'" class="slider-controller-right btn">
      <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none">
          <path d="M5 12L19 12" stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
          <path d="M12 19L19 12L12 5" stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
      </svg>
    </div>
</template>

<style scoped>
.slider-controller-left{
  display: flex;
  align-items: center;
  justify-content: center;
  width: 65px;
  height: 65px;
  background: #011627;
  border-top-left-radius: 5px;
}
.slider-controller-right{
  display: flex;
  align-items: center;
  justify-content: center;
  width: 65px;
  height: 65px;
  background: #011627;
  border-bottom-right-radius: 5px;
}
</style>