<template>
  <div>
    <div class="title">周末去哪儿</div>
    <ul>
      <li class="item border-bottom" v-for="item of weekendList" :key="item.id">
        <div class="item-img-wrapper">
          <img class="item-img" :src="item.imgUrl"/>
        </div>
        <div class="item-info">
          <p class="item-main">武陵山滑雪场</p>
          <p class="item-second">尽情体验，极致享受，干柴烈火</p>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeWeekend',
  data () {
    return {
      weekendList: [{
        id: '0001',
        imgUrl: 'https://imgs.qunarzz.com/vs_ceph_vs_tts/68a2d941-1044-47d8-bf44-9e2ab2f2902c.jpg_r_480x320x90_9944e4ed.jpg'
      }, {
        id: '0002',
        imgUrl: 'https://imgs.qunarzz.com/vs_ceph_vs_tts/68a2d941-1044-47d8-bf44-9e2ab2f2902c.jpg_r_480x320x90_9944e4ed.jpg'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
.title
  background: #eee
  line-height: .8rem
  text-indent: .2rem
  margin-top: .1rem
.item-img-wrapper
  overflow: hidden
  height: 0
  padding-bottom: 33.9%
  .item-img
    width: 100%
.item-info
  padding: .1rem
  .item-main
    font-size: .32rem
    margin-top: .1rem
    line-height: .44rem
  .item-second
    margin-top: .1rem
    color: gray
    line-height: .32rem
</style>
