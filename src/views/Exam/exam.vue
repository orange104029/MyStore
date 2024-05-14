<template>
  <div class="container">
    <div class="title">
      <hr class="hr">
      <div class="title-text">潍坊市2024小车理论考试</div>
    </div>
    <div class="content clearfix">
      <ul class="left clearfix">
        <li class="item-title">
          <a href="#">科目一交规</a>
        </li>
        <li class="item icon1">
          <a href="#">顺序练习</a>
          <p>按照顺序练习做题</p>
        </li>
        <li class="item icon2">
          <a href="#">随机练习</a>
          <p>按照随机练习做题</p>
        </li>
        <li class="item icon3">
          <a href="#">专项练习</a>
          <p>分门别类重点突破</p>
        </li>
        <li class="item icon4">
          <a href="#">难题攻克</a>
          <p>准确把握考试难点</p>
        </li>
        <li class="item-btn">
          <a href="#">模拟考试</a>
        </li>
      </ul>
      <ul class="right clearfix">
        <li class="item-title">
          <a href="#">科目四安全文明驾驶</a>
        </li>
        <li class="item icon1">
          <a href="#">顺序练习</a>
          <p>按照顺序练习做题</p>
        </li>
        <li class="item icon2">
          <a href="#">随机练习</a>
          <p>按照随机练习做题</p>
        </li>
        <li class="item icon3">
          <a href="#">专项练习</a>
          <p>分门别类重点突破</p>
        </li>
        <li class="item icon4">
          <a href="#">难题攻克</a>
          <p>准确把握考试难点</p>
        </li>
        <li class="item-btn">
          <a href="#">模拟考试</a>
        </li>
      </ul>
    </div>
    <div class="img">
      <a href="#">
        <img src="https://weifang.jiakaobaodian.com/core-assets/static/images/common/banner-jxb.png" alt="">
      </a>
    </div>
  </div>
</template>
<style scoped>
a {
  text-decoration: none;
  color: inherit;
  text-align: center;
}

a:hover {
  color: #78d0ff;
}

.container {
  width: 1200px;
  margin: 60px auto;
}

.clearfix::after {
  content: '';
  display: table;
  clear: both;
}

.img {
  width: 1200px;
  margin: 60px auto;
}

.title {
  margin-bottom: 40px;
  text-align: center;
  padding-top: 20px;
}

.hr {
  height: 1px;
  border-top: 1px dotted #e9e9e9;
}

.title-text {
  display: inline-block;
  font-size: 30px;
  margin-top: -20px;
  padding: 0 45px;
  line-height: 40px;
  background-color: #fff;
  text-align: center;
}


.content ul {
  border: 1px solid #e9e9e9;
  width: 580px;
}

.left {
  float: left;
}

.right {
  float: right;
}

.content ul li {
  list-style: none;
  padding: 0;

}

.content .item-title {
  width: 100%;
  height: 110px;
  line-height: 110px;
  padding-top: 0;
  border: none;
  margin: 0;
  text-align: center;
}

.content .item-title a {
  display: inline-block;
  padding: 0 0 0 38px;
  background: url(https://weifang.jiakaobaodian.com/core-assets/jiakao/application/home/files/cd9c3b69a1d8d0bc72b839ebdaeb5fd4.png) left center no-repeat;
  font-size: 20px;
}

.content .item {
  margin: 0 0 15px 25px;
  float: left;
  width: 250px;
  height: 70px;
  line-height: 20px;
  padding: 15px 0 15px 85px;
  background-color: #FAFAFA;
}

.item>a {
  font-size: 16px;
}

.item>p {
  color: #999;
}

.icon1 {
  background: url(https://weifang.jiakaobaodian.com/core-assets/jiakao/application/home/files/7920c46acf795cfe91990d3bb8c8635c.png) left 50px center no-repeat;

}

.icon2 {
  background: url(https://weifang.jiakaobaodian.com/core-assets/jiakao/application/home/files/29f60eac40621dffb37c38f8d584f215.png) left 50px center no-repeat;
}

.icon3 {
  background: url(https://weifang.jiakaobaodian.com/core-assets/jiakao/application/home/files/cd9c3b69a1d8d0bc72b839ebdaeb5fd4.png) left 50px center no-repeat;
}

.icon4 {
  background: url(https://weifang.jiakaobaodian.com/core-assets/jiakao/application/home/files/f117d8ae0fca3bffd25ff4511664e607.png) left 50px center no-repeat;
}

.content .item-btn {
  width: 100%;
  overflow: hidden;
  float: right;
}

.content .item-btn>a {
  width: 300px;
  height: 46px;
  line-height: 46px;
  margin: 15px auto 30px;
  display: block;
  background: #37B5F8;
  color: #fff;
  border-radius: 4px;

}
</style>