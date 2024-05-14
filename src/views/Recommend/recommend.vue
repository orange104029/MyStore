<template>
  <div class="container">
    <div class="title">
      <hr class="hr">
      <div class="title-text">潍坊市驾校推荐</div>
    </div>
    <div>
      <ul class="school-list clearfix">
        <li>
          <div class="item-top clearfix">
            <div class="col1 left">
              <div class="div1">
                <span class="name">学府驾校</span>

                <div class="star"></div>

              </div>
              <div class="div2">
                <span>口碑好</span>
                <span>规模大</span>
                <span>拿本快</span>
                <span>包接送</span>
              </div>
            </div>
            <div class="col2 left">
              <p class="price">￥3370</p>
            </div>
            <div class="col3 right">
              <button class="btn">学车报名</button>
            </div>
          </div>
          <div class="item-content">
            <div class="img">
              <img src="https://avatar-user.mucang.cn/user-avatar/default/U7i271K6lUs.jpg!100x100" alt="">
            </div>
            <p class="content">刘教练很有耐心，不会凶学员也很细心，是个好教练</p>
          </div>
        </li>
        <li>
          <div class="item-top clearfix">
            <div class="col1 left">
              <div class="div1">
                <span class="name">宏翔驾校</span>

                <div class="star"></div>

              </div>
              <div class="div2">
                <span>口碑好</span>
                <span>规模大</span>
                <span>拿本快</span>
                <span>包接送</span>
              </div>
            </div>
            <div class="col2 left">
              <p class="price">￥3770</p>
            </div>
            <div class="col3 right">
              <button class="btn">学车报名</button>
            </div>
          </div>
          <div class="item-content">
            <div class="img">
              <img src="https://avatar-user.mucang.cn/user-avatar/default/U7i271K6lUs.jpg!100x100" alt="">
            </div>
            <p class="content">教练差劲 服务态度：不好教练不管</p>
          </div>
        </li>
        <li>
          <div class="item-top clearfix">
            <div class="col1 left">
              <div class="div1">
                <span class="name">瑞达驾校</span>

                <div class="star"></div>

              </div>
              <div class="div2">
                <span>口碑好</span>
                <span>规模大</span>
                <span>拿本快</span>
                <span>包接送</span>
              </div>
            </div>
            <div class="col2 left">
              <p class="price">￥2770</p>
            </div>
            <div class="col3 right">
              <button class="btn">学车报名</button>
            </div>
          </div>
          <div class="item-content">
            <div class="img">
              <img src="https://avatar-user.mucang.cn/user-avatar/default/U7i271K6lUs.jpg!100x100" alt="">
            </div>
            <p class="content">服务态度：很好 学车体验：很好 通过率：高 规范收费：透明收费</p>
          </div>
        </li>
        <li>
          <div class="item-top clearfix">
            <div class="col1 left">
              <div class="div1">
                <span class="name">潍坊职业学院驾校</span>

                <div class="star"></div>

              </div>
              <div class="div2">
                <span>口碑好</span>
                <span>规模大</span>
                <span>拿本快</span>
                <span>包接送</span>
              </div>
            </div>
            <div class="col2 left">
              <p class="price">￥2770</p>
            </div>
            <div class="col3 right">
              <button class="btn">学车报名</button>
            </div>
          </div>
          <div class="item-content">
            <div class="img">
              <img src="https://avatar-user.mucang.cn/user-avatar/default/U7i271K6lUs.jpg!100x100" alt="">
            </div>
            <p class="content">驾校很nice，教练很nice</p>
          </div>
        </li>
      </ul>

      <div class="more">
        <a href="#">查看更多</a>
      </div>
    </div>

  </div>
</template>
<style scoped>
a {
  text-decoration: none;
  color: inherit;
  text-align: center;
}

li {
  list-style: none;
}

.clearfix::after {
  content: '';
  display: table;
  clear: both;
}

.container {
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

.school-list {
  margin: -30px 0 0 -30px;
  color: #666;
  font-size: 14px;
}

.school-list>li {
  float: left;
  position: relative;
  width: 585px;
  margin: 30px 0 0 30px;
  padding: 40px 30px;
  border: 1px solid #e9e9e9;
}

.left {
  float: left;
}

.right {
  float: right;
}

.col1 {
  width: 305px;
  line-height: 30px;
}

.col1 .div1 .name {
  display: inline-block;
  vertical-align: middle;
  font-size: 22px;
  /* overflow: hidden; */
}

.col1 .div1 .star {
  display: inline-block;
  vertical-align: middle;
  margin: -3px 0 0 10px;
  width: 90px;
  height: 20px;
  background: url(https://weifang.jiakaobaodian.com/core-assets/jiakao/application/home/files/26170a2c1308047cbc25d47cc860cd1e.png) left center no-repeat;
}

.col1 .div2 {
  margin-top: 10px;
  line-height: 20px;
}

.col1 .div2 span {
  display: inline-block;
  background: url(https://weifang.jiakaobaodian.com/core-assets/jiakao/application/home/files/24bc3d8a827f32b86d0ed191681125f9.png) left center no-repeat;
  padding-left: 20px;
}

.col1 .div2>span+span {
  margin-left: 10px;
}

.col2 {
  width: 130px;
  line-height: 63px;
  border-left: 1px solid #e9e9e9;
  font-size: 30px;
  text-align: center;
}

.price {
  color: #EE4653;
}

.col3 .btn {
  width: 80px;
  line-height: 28px;
  margin-top: 17px;
  text-align: center;
  font-size: 14px;
  border-radius: 4px;
  border: 1px solid #e9e9e9;
  background: 0 0;
}

.item-content {
  height: 80px;
  margin-top: 30px;
  padding: 20px;
  background: #FAFAFA;
  color: #999;
}

.item-content .img img {
  float: left;
  width: 40px;
  height: 40px;
}

.item-content .content {
  height: 40px;
  line-height: 20px;
  margin-left: 60px;
}

.more {
  margin-top: 40px;
}

.more a {
  display: block;
  width: 280px;
  margin: 20px auto 0;
  line-height: 48px;
  border: 1px solid #e9e9e9;
  border-radius: 4px;
  color: #999;
  text-align: center;
  font-size: 16px;
}
</style>