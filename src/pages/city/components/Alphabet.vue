<template>
  <div class="item-list">
    <div class="item" v-for="(item,key) of cities" :key="key">{{key}}</div>
  </div>
</template>

<script>
export default {
  name: 'CityAlphabet',
  props: {
    cities: Object
  }
}
</script>

<style lang="stylus" scoped>
.item-list
  display: flex
  flex-direction: column
  justify-content: center
  position: absolute
  top: 1.58rem
  right: 0
  bottom: 0
  width: .4rem
  .item
    text-align: center
    color: #00bcd4
    line-height: .4rem
</style>
