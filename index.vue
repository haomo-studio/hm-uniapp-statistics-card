<template>
  <div class="hm-statistics-card">
    <div class="overall">
      <div class="head">
        <text class="title">{{ options.title }}</text>
        <image class="titleImg" :src="options.titleImg" />
      </div>
      <div class="typeClass">
        <div class="type" />
        <text class="access">{{ options.access }}</text>
        <div class="secondTypes" />
        <text class="sales">{{ options.sales }}</text>
        <div class="thirdTypes" />
        <text class="revenue">{{ options.revenue }}</text>
      </div>
      <div class="body">
        <div class="bgWrap">
          <image class="picimg" :src="options.picimg" />
          <image class="itemimg" :src="options.itemimg" />
          <image class="layerimg" :src="options.layerimg" />
          <image class="img" :src="options.img" />
          <image class="productimg" :src="options.productimg" />
          <image class="bgimg" :src="options.bgimg" />
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'HmStatisticsCard',
  props: {
    dataId: {
      type: String,
      default: 'hm-statistics-card'
    },
    options: {
      type: Object,
      default: function() {
        return {
          title: '统计',
          titleImg:
            './images/img_24239_0_1.png',
          access: '访问',
          sales: '销售额',
          revenue: '收益',
          picimg:
            './images/img_24239_0_2.png',
          itemimg:
            './images/img_24239_0_3.png',
          layerimg:
            './images/img_24239_0_4.png',
          img:
            './images/img_24239_0_5.png',
          productimg:
            './images/img_24239_0_6.png',
          bgimg:
            './images/img_24239_0_0.png'
        };
      }
    }
  },
  data() {
    return {};
  },
  methods: {}
};
</script>
<style>
@import './index.response.css';
</style>
