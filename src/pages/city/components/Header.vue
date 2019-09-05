<template>
  <div class="header">
    城市选择
    <router-link to="/">
      <span class="iconfont icon">&#xe624;</span>
    </router-link>
  </div>
</template>

<script>
export default {
  name: 'CityHeader'
}
</script>

<style lang="stylus" scoped>
.header
  position: relative
  overflow: hidden
  background: #00bcd4
  height: .86rem
  line-height: .86rem
  text-align: center
  font-size: .32rem
  color: #fff
  .icon
    position: absolute
    left: 0
    top: 0
    margin-left: .2rem
    font-size: .32rem
    color: #fff
</style>
