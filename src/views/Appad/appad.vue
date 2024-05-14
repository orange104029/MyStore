<template>
  <div class="appad">
    <div class="content">
      <div class="ad1">
        <span>教练宝典APP</span>
        <div></div>
      </div>
      <div class="ad2">
        <span>驾考宝典APP</span>
        <div></div>
      </div>
      <div class="ad3">
        <span>买车宝典APP</span>
        <div></div>
      </div>
    </div>
  </div>
  <div class="app-down">
    <ul class="item clearfix">
      <li class="left">
        <span>驾考宝典APP下载</span>
        <p>考驾照 用宝典</p>
      </li>
      <li class="left right">
        <span>驾考宝典微信小程序</span>
        <p>无需下载，驾考做题更方便！</p>
      </li>
    </ul>

  </div>
</template>
<style scoped>
.clearfix::after {
  content: '';
  display: table;
  clear: both;
}

li {
  list-style: none;
}

.appad {
  background-color: #f5f5f5;
}

.content {
  position: relative;
  width: 1200px;
  height: 560px;
  margin: 70px auto 0;
  overflow: hidden;
}

.content>div {
  position: absolute;
  bottom: -40px;
  text-align: center;
}

.content>div span {
  font-size: 20px;
}

.content .ad1 {
  left: 30px;
  width: 300px;
  height: 500px;
  background: url(https://weifang.jiakaobaodian.com/core-assets/jiakao/application/home/files/f4b3be31a83c5d02bf5cb2e0fb11636b.png) center bottom no-repeat;
  transition: transform 0.8s ease;
}

.content .ad1>div {
  display: none;
  width: 100%;
  height: 100%;
  margin-top: 37px;
  background: url(https://weifang.jiakaobaodian.com/core-assets/jiakao/application/home/files/2d1920df784226626de9efd062e808a2.png) center no-repeat;

}

.ad1:hover div {
  display: block;
}

.ad1:hover {
  transform: translateY(-40px);
}

.content .ad2 {
  left: 400px;
  width: 430px;
  height: 540px;
  background: url(https://weifang.jiakaobaodian.com/core-assets/jiakao/application/home/files/48726c2bb302051522dfc028c0532488.png) center bottom no-repeat;
  transition: transform 0.8s ease;
}

.content .ad2>div {
  display: none;
  width: 100%;
  height: 100%;
  margin-top: 52px;
  background: url(https://weifang.jiakaobaodian.com/core-assets/jiakao/application/home/files/47b4a64f54ae7eaace0daaf9dc3446c5.png) center no-repeat;
  background-color: rgba(255, 255, 255, .5);
  background-size: 150px 150px;
}

.ad2:hover div {
  display: block;
}

.ad2:hover {
  transform: translateY(-40px);
}

.content .ad3 {
  left: 905px;
  width: 265px;
  height: 428px;
  background: url(https://weifang.jiakaobaodian.com/core-assets/jiakao/application/home/files/40ab1d6a3ed0757b51ad19cbec3b29c4.png) center bottom no-repeat;
  transition: transform 0.8s ease;
}

.content .ad3>div {
  display: none;
  width: 100%;
  height: 100%;
  margin-top: 37px;
  background: url(https://weifang.jiakaobaodian.com/core-assets/jiakao/application/home/files/188c7ffa5035c0976ff6e06a1ca89666.png) center no-repeat;

}

.ad3:hover div {
  display: block;
}

.ad3:hover {
  transform: translateY(-40px);
}

.app-down {
  width: 1200px;
  margin: 60px auto;
}

.left {
  float: left;
  width: 600px;
  line-height: 1.7;
  margin: 20px 0;
  padding: 40px 80px;
  background: url(https://weifang.jiakaobaodian.com/core-assets/jiakao/application/home/files/dd59a20c70d3f6ed409efc01c65ad14d.png) right 80px center no-repeat;
  background-size: 140px;
  border-right: 1px solid #e9e9e9;
}

.left>span {
  font-size: 20px;
}

.item .right {
  float: right;
  background: url(https://weifang.jiakaobaodian.com/core-assets/jiakao/application/home/files/9e699ddb2a6e87f8fbe90aa6b1d01564.jpg) right 80px center no-repeat;
  background-size: 130px;
  border: none;
}
</style>