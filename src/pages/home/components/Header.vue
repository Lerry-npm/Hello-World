<template>
  <div class="header">
    <div class="header-left">
      <div class="iconfont back-icon">&#xe624;</div>
    </div>
    <div class="header-input">
      <span class="iconfont">&#xe632;</span>
      输入城市，游玩景点
    </div>
    <router-link to="/city">
      <div class="header-right">
        {{this.city}}
        <span class="iconfont arrow-icon">&#xe64a;</span>
      </div>
    </router-link>
  </div>
</template>

<script>
export default {
  name: 'HomeHeader',
  props: {
    city: String
  }
}
</script>

<style lang='stylus' scoped>
@import '~styles/varibles.styl'
.header
  display: flex
  line-height: .86rem
  background: $bgColor
  color: #fff
  .header-left
    float: left
    width: .64rem
    .back-icon
      font-size: .4rem
      text-align: center
  .header-input
    flex: 1
    height: .64rem
    line-height: .64rem
    margin-left: .2rem
    margin-top: .12rem
    padding-left: .2rem
    background: #fff
    color: #ccc
    border-radius: .1rem
  .header-right
    float: right
    width: 1.24rem
    text-align: center
    .arrow-icon
      font-size: .24rem
      color: #fff
</style>
