<template>
  <div class="search">
    <input class="search-input" type="text" placeholder="输入城市名或拼音"/>
  </div>
</template>

<script>
export default {
  name: 'CitySearch'
}
</script>

<style lang="stylus" scoped>
.search
  background: #00bcd4
  height: .72rem
  line-height: .72rem
  padding: 0 .1rem
  .search-input
    box-sizing: border-box
    width: 100%
    height: .6rem
    line-height: .6rem
    padding: 0 .1rem
    text-align: center
    border-radius: .06rem
    color: #666
</style>
