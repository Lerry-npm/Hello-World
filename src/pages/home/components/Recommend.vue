<template>
  <div>
    <div class="title">热销推荐</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <img class="item-img" :src="item.imgUrl"/>
        <div class="item-info">
          <p class="item-main">大连游泳馆</p>
          <p class="item-second">畅游海洋，亲友团聚，共聚一堂</p>
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
        imgUrl: 'https://imgs.qunarzz.com/vs_ceph_vs_tts/d2fd1bcb-1ce3-427e-a61c-7c0c41c2196a.jpg_r_390x260x90_733fb20e.jpg'
      }, {
        id: '0002',
        imgUrl: 'https://imgs.qunarzz.com/vs_ceph_vs_tts/d2fd1bcb-1ce3-427e-a61c-7c0c41c2196a.jpg_r_390x260x90_733fb20e.jpg'
      }, {
        id: '0003',
        imgUrl: 'https://imgs.qunarzz.com/vs_ceph_vs_tts/d2fd1bcb-1ce3-427e-a61c-7c0c41c2196a.jpg_r_390x260x90_733fb20e.jpg'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
.title
  background: #eee
  margin-top: .16rem
  line-height: .8rem
  text-indent: .2rem
.item
  display: flex
  overflow: hidden
  height: 1.9rem
  .item-img
    height: 1.7rem
    width: 1.7rem
    padding: .1rem
  .item-info
    flex: 1
    padding: .1rem
    .item-main
      font-size: .32rem
      line-height: .54rem
    .item-second
      line-height: .4rem
      color: #ccc
    .item-button
      line-height: .44rem
      margin-top: .16rem
      background: #ff9300
      padding: 0 .2rem
      border-radius: .06rem
      color: #fff
</style>
