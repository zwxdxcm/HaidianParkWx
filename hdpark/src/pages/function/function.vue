<template>
  <view>
    <uni-section title="功能简述" type="circle"></uni-section>
    <text class = "txt">功能: 1.寻找附近探险地点 2.定制我的出游计划</text>
    <uni-section title="地图api" type="circle"></uni-section>
    <view style="margin:20rpx">
      <map
        style="width: 100%; height: 300px;"
        :latitude="latitude"
        :longitude="longitude"
        :markers="covers"
      ></map>
    </view>
  </view>
</template>

<script>
import uniSection from "@/components/uni-section/uni-section.vue";
export default {
  name: "",
  components: { uniSection },
  data() {
    return {
      id: 0, // 使用 marker点击事件 需要填写id
      title: "map",
      latitude: 39.909,
      longitude: 116.39742,
      covers: [
        {
          latitude: 39.909,
          longitude: 116.39742
        },
        {
          latitude: 39.9,
          longitude: 116.39
        }
      ]
    };
  }
};
</script>

<style >
.txt {
  display: block;
  font-size: 16px;
  line-height: 20px;
}
</style>