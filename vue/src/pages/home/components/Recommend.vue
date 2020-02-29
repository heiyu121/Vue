<template>
  <div>
    <div class="title">热销推荐</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <img class="item-img" :src="item.imgUrl" />
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{item.desc}}</p>
          <button class="item-button">查看详情</button>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeRecommend',
  data () {
    return {
      recommendList: [{
        id: '0001',
        imgUrl: 'https://imgs.qunarzz.com/sight/p0/1708/2b/2b3b94de99c0a425a3.img.jpg_250x250_50c99cf3.jpg',
        title: '暂无说明',
        desc: '暂无说明'
      }, {
        id: '0002',
        imgUrl: 'https://imgs.qunarzz.com/sight/p0/1708/2b/2b3b94de99c0a425a3.img.jpg_250x250_50c99cf3.jpg',
        title: '暂无说明',
        desc: '暂无说明'
      }, {
        id: '0003',
        imgUrl: 'https://imgs.qunarzz.com/sight/p0/1708/2b/2b3b94de99c0a425a3.img.jpg_250x250_50c99cf3.jpg',
        title: '暂无说明',
        desc: '暂无说明'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/mixins.styl'
  .title
    margin-top: .2rem
    line-height : .8rem
    background : #EEEEEE
    text-indent : .2rem
  .item
    overflow : hidden
    display: flex
    height : 1.9rem
    .item-img
      width: 1.7rem
      height : 1.7rem
      padding : .1rem
    .item-info
      flex: 1
      padding : .1rem
      min-width: 0
      .item-title
        line-height: .54rem
        font-size: .32rem
        ellipsis()
      .item-desc
        line-height : .4rem
        color: #CCCCCC
        ellipsis()
      .item-button
        line-height : .44rem
        margin-top .16rem
        background : #ff9300
        padding : 0 .1rem
        border-radius: .06rem
        color: #FFFFFF
</style>
