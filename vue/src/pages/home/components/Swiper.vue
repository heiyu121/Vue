<template>
  <div class="wrapper">
    <swiper :options="swiperOption">
        <swiper-slide v-for="item of swiperList" :key="item.id">
          <img class="swiper-img" :src="item.imgUrl" />
        </swiper-slide>
        <div class="swiper-pagination"  slot="pagination"></div>
      </swiper>
    </div>
</template>

<script>

export default {
  name: 'HomeSwiper',
  data () {
    return {
      // 有错误，轮播的点出不来
      swiperOption: {
        pagination: {
          el: '.swiper-pagination',
          clickable: true
        },
        loop: true
      },
      swiperList: [{
        id: '0001',
        imgUrl: 'https://img1.qunarzz.com/qs/1912/96/2c110e7b64063502.jpg'
      }, {
        id: '0002',
        imgUrl: 'https://img1.qunarzz.com/qs/2001/d3/2859c13f92a45202.jpg'
      }
      ]
    }
  }
}
</script>

<style lang="stylus" scoped>
  .wrapper>>> .swiper-pagination-bullet-active
    background: #fff;
  .wrapper
    overflow: hidden
    width: 100%
    height: 0
    padding-bottom : 31.25%
    background : #eee
    .swiper-img
      width : 100%
</style>
