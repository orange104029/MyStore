<script setup>
import { ref } from 'vue';

const links = ref([
  { text: '首页', active: true },
  {
    text: '模拟考试',
    active: false,
    dpcon: [
      '科目一',
      '科目二',
      '科目三',
      '科目四'
    ]
  },
  {
    text: '找驾校',
    active: false,
    dpcon: [
      '找驾校',
      '找教练',
      '找陪练'
    ]
  },
  { text: '驾考圈', active: false },
  { text: '交通标志', active: false },
  { text: '软件下载', active: false },
  { text: '驾考宝典企业版', active: false },
  { text: '智慧驾校', active: false },
  {
    text: '买新车',
    active: false,
    dpcon: [
      '买车网',
      '平行之家'
    ]
  },
  { text: '二手车', active: false },
])

const handleClick = (clickedlink) => {
  links.value.forEach(link => {
    link.active = (link.text === clickedlink.text)
  });
}
</script>

<template>
  <div class="header">
    <div class="nav-top">
      <div class="logo">
        <a href="https://www.jiakaobaodian.com/"></a>
      </div>
      <div class="search">
        <input type="text" placeholder="请输入关键字">
        <button>搜 索</button>
      </div>
    </div>

    <div class="nav-link">
      <ul>
        <li v-for="(link, index) in links" :key="index">
          <a :class="{ active: link.active, 'special-width': index === 6 }" @click="handleClick(link)" href="#">{{
            link.text }}{{ link.dpcon ? '▼' : '' }}</a>

          <div v-if="link.dpcon" class="dropdown-content">
            <a v-for="item in link.dpcon" href="#">{{ item }}</a>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>
<style scoped>
.header {
  display: flex;
  flex-direction: column;
}

.nav-top {
  width: 1200px;
  height: 42px;
  margin: 28px auto;
  overflow: hidden;
}

.logo {
  width: 207px;
  height: 100%;
  float: left;
}

.logo a {
  width: 207px;
  height: 100%;
  display: block;
  background: url(https://weifang.jiakaobaodian.com/core-assets/jiakao/application/home/files/8db7d0f8978fcfd464f665b2ed7a54a2.png) left center no-repeat;
}

.search {
  width: 300px;
  height: 42px;
  float: right;
}

.search input {
  width: 80%;
  height: 100%;
  border: 1px solid #e9e9e9;
  color: #525252;
  font-size: 14px;
  /* padding-left: 10px; */
  border-radius: 0px;
}

.search input:focus {
  border-color: #37B5F8;
  /* 设置选中时的边框颜色 */
  outline: none;
}

.search button {
  width: 20%;
  height: 100%;
  border: 1px solid #e9e9e9;
  font-size: 14px;
  border-radius: 0px;
}

.nav-link {
  width: 100%;
  background-color: #37B5F8;
  color: white;
  position: relative;
}

.nav-link ul {
  width: 1200px;
  height: 50px;
  margin: auto;
  padding: 0;
  align-items: center;
  /* 垂直居中子元素 */
}

.nav-link li {
  display: inline-block;
}

.nav-link a {
  display: block;
  width: 108px;
  height: 50px;
  text-align: center;
  line-height: 50px;
  text-decoration: none;
  color: white;
}

.nav-link a.special-width {
  width: 148px;
  /* 设置特定宽度 */
}

.nav-link a.active {
  background-color: #258FC7;
}

.nav-link a:not(.active):hover {
  background-color: #78d0ff;
}

.nav-link li:hover .dropdown-content {
  display: block;
}

.nav-link .dropdown-content {
  display: none;
  position: absolute;
  top: 50px;
  z-index: 2;
  font-size: 14px;
  background-color: white;
}

.nav-link .dropdown-content a {
  height: 100%;
  line-height: 40px;
  color: black;
  padding: 0 8px;
}

.nav-link .dropdown-content a:hover {
  color: #78d0ff;
  background-color: white;
}
</style>