<template>
  <view>
    <!-- <img src="static/hdlogo.jpg" class="logo" /> -->
    <uni-card
      title="海淀公园"
      mode="title"
      thumbnail="https://hdpark.oss-cn-beijing.aliyuncs.com/hdlogo.jpg"
      :is-shadow="true"
      extra="HD PARK"
    >
      <view>
        <view class="img-container">
          <img src="https://hdpark.oss-cn-beijing.aliyuncs.com/hd-intro.jpg" class="pic" />
        </view>
        <view class="txt-container">
          <text
            class="txt"
          >海淀公园是一组来自中国海淀的摇滚-探险乐队。由乐队主唱布鲁恩斯坦-朝伟翔-上庄籍主音，犇洛特利-Gin-丰台籍DJ-，GinWANG-张-上地籍键盘手、Angela-腿祺-美籍吉祥物组成。</text>
        </view>
      </view>
    </uni-card>
    <uni-card title="成员介绍" mode="basic" :is-shadow="true">
      <view class="intro-pic-container">
        <view class="img-container">
          <image
            src="https://hdpark.oss-cn-beijing.aliyuncs.com/zwx.png"
            mode="aspectFill"
            class="intro-pic"
          />
        </view>
        <view class="img-container">
          <image
            src="https://hdpark.oss-cn-beijing.aliyuncs.com/zzn.png"
            mode="aspectFill"
            class="intro-pic"
          />
        </view>
        <view class="img-container">
          <image
            src="https://hdpark.oss-cn-beijing.aliyuncs.com/yb.png"
            mode="aspectFill"
            class="intro-pic"
          />
        </view>
        <view class="img-container">
          <image
            src="https://hdpark.oss-cn-beijing.aliyuncs.com/wjq2.png"
            mode="aspectFill"
            class="intro-pic"
          />
        </view>
      </view>
    </uni-card>
  </view>
</template>

<script>
import uniCard from "@/components/uni-card/uni-card.vue";
export default {
  name: "",
  data() {
    return {};
  },
  components: { uniCard }
};
</script>

<style >
.img-container {
  display: flex;
  justify-content: center;
  margin:10rpx
}
.pic {
  height: 400rpx;
  width: 600rpx;
}
.txt-container {
  padding: 20rpx;
}
.txt {
  display: block;
  font-size: 14px;
  line-height: 20px;
}
.intro-pic-container {
  display: flex;
  justify-content: space-around;

}
.intro-pic {
  height: 400rpx;
  width: 150rpx;
}
</style>