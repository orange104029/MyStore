<script setup>
import { onMounted, ref } from 'vue';
const slides = [
  { image: 'https://weifang.jiakaobaodian.com/core-assets/static/images/common/home_banner_download.png' },
  { image: 'https://weifang.jiakaobaodian.com/core-assets/static/images/common/home_banner_new1.jpeg' },
  { image: 'https://weifang.jiakaobaodian.com/core-assets/static/images/common/home_banner_jiaolian.jpg' },
  { image: 'https://weifang.jiakaobaodian.com/core-assets/static/images/common/home_banner_jiaxiaobang.png' }
]
const currentIndex = ref(0);

const slidesContainer = ref(null);
let nextSlide = null

const startAutoSwitch = () => {
  nextSlide = setInterval(() => {
    currentIndex.value = (currentIndex.value + 1) % slides.length;
    console.log(currentIndex.value);
  }, 5000)
}
const stopAutoSwitch = () => {
  clearInterval(nextSlide);
  nextSlide = null;
}
const goToSlide = (index) => {
  currentIndex.value = index;
};
// onMounted(() => nextSlide())
</script>
<template>
  <div class="carousel">
    <div class="slides" ref="slidesContainer" :style="{ transform: `translateX(-${currentIndex * 100}%)` }"
      @mouseover="stopAutoSwitch" @mouseout="startAutoSwitch">
      <div v-for="(slide, index) in slides" :key="index" class="slide">
        <img :src="slide.image" alt="slide">
      </div>
    </div>
    <div class="dots">
      <span v-for="(slide, index) in slides" :key="index" :class="{ active: index === currentIndex }"
        @click="goToSlide(index)"></span>
    </div>
    <div class="menu-container">
      <div class="menu">
        <p class="menu-title">学车流程</p>
        <ul class="menu-list">
          <li class="icon1">
            <p class="p1">
              <a href="#">科目一</a>
            </p>
            <p class="p2">2024新题库</p>
          </li>
          <li class="icon2">
            <p class="p1">
              <a href="#">科目二</a>
            </p>
            <p class="p2">精选视频，详解考点</p>
          </li>
          <li class="icon3">
            <p class="p1">
              <a href="#">科目三</a>
            </p>
            <p class="p2">全方位讲解，攻克难点</p>
          </li>
          <li class="icon4">
            <p class="p1">
              <a href="#">科目四</a>
            </p>
            <p class="p2">2024新题库</p>
          </li>
        </ul>
      </div>

    </div>
  </div>
</template>
<style scoped>
a {
  text-decoration: none;
  color: inherit;
}

li {
  list-style: none;
}

.carousel {
  position: relative;
  width: 1707px;
  height: 380px;
  background-color: aquamarine;
  overflow: hidden;
}

.slides {
  width: 100%;
  height: 380px;
  display: flex;
  transition: transform 0.5s ease;
  /* 添加平滑过渡效果 */
}

.slide {
  flex: 0 0 100%;
  /* 每张图片宽度为100% */
}

.slide img {
  max-width: 100%;
  height: 380px;
  margin: 0 auto;
}


.dots {
  position: absolute;
  bottom: 10px;
  left: 50%;
  transform: translateX(-50%);
  display: flex;
}

.dots span {
  width: 8px;
  height: 8px;
  border-radius: 50%;
  background-color: #ccc;
  margin: 0 5px;
  cursor: pointer;
}

.dots span.active {
  background-color: #007aff;
}

.menu-container {
  position: relative;
  width: 1200px;
  height: 0;
  margin: 0 auto;
  overflow: visible;
}

.menu {
  position: absolute;
  top: -358px;
  left: 0;
  width: 280px;
  z-index: 1;
  padding: 0 20px;
  background-color: rgba(255, 255, 255, .9);
}

.menu-title {
  line-height: 50px;
  font-size: 20px;
  border-bottom: 1px dotted #ddd;
  text-align: center;
}

.menu>.menu-list>li {
  height: 72px;
  padding: 18px 20px 18px 50px;
}

.menu>.menu-list .icon1 {
  background: url(https://weifang.jiakaobaodian.com/core-assets/jiakao/application/home/files/967c5f51b9995b3cea6ac917ccebbd10.png) left center no-repeat;
}

.menu>.menu-list .icon2 {
  background: url(https://weifang.jiakaobaodian.com/core-assets/jiakao/application/home/files/9bfc61e92388bf9d0521dbbc5497172b.png) left center no-repeat;
}

.menu>.menu-list .icon3 {
  background: url(https://weifang.jiakaobaodian.com/core-assets/jiakao/application/home/files/5061edda4ba913bd8f1ca5bdaee8d1d7.png) left center no-repeat;
}

.menu>.menu-list .icon4 {
  background: url(https://weifang.jiakaobaodian.com/core-assets/jiakao/application/home/files/ef73328f70c08beb91f54eae709a05b1.png) left center no-repeat;
}

.menu>.menu-list>li>.p1 {
  color: #37B5F8;
  font-size: 16px;
}

.menu>.menu-list>li>.p2 {
  font-size: 14px;
  margin-top: 5px;
  color: #666;
}
</style>