<script setup lang="ts">
import TestimonialComponent from '@/components/testimonial-component.vue'
</script>
<template>
    <div class="container-box">
        <div class="line"></div>
        <div class="people-thought-box">
            <div class="header">
                <div class="title m-b-31">People’s thoughts</div>
                <div class="title2">SEE WHAT ARE OTHERS SAYING</div>
            </div>
            <div class="body">
                <div v-for="index in 4" :key="index">
                    <TestimonialComponent class="m-r-24 m-b-24"/>
                </div>
            </div>
        </div>
        <div class="footer">
            <div class="title m-b-31">See you soon!</div>
            <div class="title3">We hope to meet each other very soon.</div>
        </div>
        <div class="line-bottom"></div>
    </div>
</template>

<style scoped>
.container-box{
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    margin: 235px 120px 138px 120px;
    width: 1680px;
    height: 1710px;
    flex-shrink: 0;
}
.body{
    display: flex; 
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;
    width: 1144px;
}
.people-thought-box{
    width: 1680px;
    height: 1448px;
    flex-shrink: 0;
    border-radius: 8px;
    background: #011627;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
}
.title{
    color: #FFF;
    text-align: center;
    font-family: 'Noe Display';
    font-size: 72px;
    font-style: normal;
    font-weight: 700;
    line-height: 110%; /* 79.2px */
    letter-spacing: -1.44px;
}
.title2{
    color: #FFF;
    text-align: center;
    font-family: 'Larsseit' sans-serif;
    font-size: 24px;
    font-style: normal;
    font-weight: 700;
    line-height: 150%; /* 36px */
    letter-spacing: 3.6px;
}
.title3{
    color: #FFF;
    text-align: center;
    font-family: 'Larsseit' sans-serif;
    font-size: 24px;
    font-style: normal;
    font-weight: 700;
    line-height: 150%; /* 36px */
    letter-spacing: 1.68px;
    flex-shrink: 0;
}
.header{
    width: 545px;
    height: 143px;
    flex-shrink: 0;
    margin-top: 60px;
    margin-bottom: 73px;
}
.line{
    width: 2px;
    height: 80px;
    flex-shrink: 0;
    border-radius: 13px;
    background: linear-gradient(180deg, #09F4F4 0%, #00C9E0 100%);
    margin-top: -85px;
}
.line-bottom{
    width: 2px;
    height: 80px;
    flex-shrink: 0;
    border-radius: 13px;
    background: linear-gradient(180deg, #09F4F4 0%, #00C9E0 100%);
    margin-top: 138px;
}
.footer{
    width: 424px;
    height: 172px;
    flex-shrink: 0;
    text-align: center;
}
</style>