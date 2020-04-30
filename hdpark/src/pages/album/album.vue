<template>
  <view>
    <uni-section title="G2016五班" type="circle"></uni-section>
    <uni-swiper-dot
      :info="info"
      current="0"
      mode="default"
      :dots-styles="dotsStyles"
      field="content"
    >
      <swiper class="swiper-box" @change="change">
        <swiper-item v-for="(item, index) in info" :key="index">
          <view :class="item.colorClass" class="swiper-item">
            <image :src="item.url" class="image" mode="aspectFill" />
          </view>
        </swiper-item>
      </swiper>
    </uni-swiper-dot>
    <uni-section title="上海巡演" type="circle"></uni-section>
    <uni-section title="云南巡演" type="circle"></uni-section>
    <uni-section title="斯里兰卡巡演" type="circle"></uni-section>
    <uni-section title="菲律宾巡演" type="circle"></uni-section>
  </view>
</template>

<script>
import uniSection from "@/components/uni-section/uni-section.vue";
import uniSwiperDot from "@/components/uni-swiper-dot/uni-swiper-dot.vue";
export default {
  name: "",
  components: { uniSection, uniSwiperDot },
  data() {
    return {
      info: [
        {
          url: "https://hdpark.oss-cn-beijing.aliyuncs.com/g05/g501.png",
          content: "内容 A"
        },
        {
          url: "https://hdpark.oss-cn-beijing.aliyuncs.com/g05/g502.png",
          content: "内容 B"
        },
        {
          url: "https://hdpark.oss-cn-beijing.aliyuncs.com/g05/g503.png",
          content: "内容 C"
        }
      ]
    };
  },

  methods: {
    change(e) {
      this.current = e.detail.current;
    }
  }
};
</script>

<style >
.swiper-item {
  display: flex;

  justify-content: center;
  align-items: center;
  background-color: #999;
  color: #fff;
}
.swiper-box {
  height: 200px;
}

.image {
  width: 750rpx;
}
</style>