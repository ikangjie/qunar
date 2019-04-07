<template>
  <div>
    <div class="title">周末去哪</div>
    <ul>
      <li class="item" v-for="item of recommendList" :key="item.id">
        <div class="item-img-wrapper">
          <img class="item-img" :src="item.imgUrl" />
        </div>
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{item.desc}}</p>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'Weekend',
  data () {
    return {
      recommendList: [{
        id: '001',
        imgUrl: 'http://img1.qunarzz.com/sight/source/1505/9f/f585152825459.jpg_r_640x214_5d46e4cc.jpg',
        title: '大连圣亚海洋世界1',
        desc: '浪漫大连首战，浪漫的海洋主题乐园'
      }, {
        id: '002',
        imgUrl: 'http://img1.qunarzz.com/sight/source/1505/9f/f585152825459.jpg_r_640x214_5d46e4cc.jpg',
        title: '大连圣亚海洋世界2',
        desc: '浪漫大连首战，浪漫的海洋主题乐园'
      }, {
        id: '003',
        imgUrl: 'http://img1.qunarzz.com/sight/source/1505/9f/f585152825459.jpg_r_640x214_5d46e4cc.jpg',
        title: '大连圣亚海洋世界3',
        desc: '浪漫大连首战，浪漫的海洋主题乐园'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/mixins.styl'
  .title
    margin-top .2rem
    line-height .8rem
    text-indent .2rem
    background #eee
  .item-img-wrapper
    overflow hidden
    height 0
    padding-bottom 33.9%
    .item-img
      width 100%
  .item-info
    padding .1rem
    .item-title
      line-height .54rem
      font-size .32rem
      ellipsis()
    .item-desc
      line-height .4rem
      color #ccc
      ellipsis()
</style>
