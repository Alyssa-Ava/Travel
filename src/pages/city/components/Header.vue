<template>
  <div class="city-header">
    <div class="iconfont back-icon">&#xe624;</div>
    城市选择
  </div>
</template>

<script>
export default {
  name: 'cityHeader'
}
</script>

<style lang="stylus" scoped>
  @import '~styles/varibles.styl'
  .city-header
    height $headerHeight
    line-height $headerHeight
    overflow hidden
    position relative
    font-size .32rem
    text-align center
    background $bgColor
    color #fff
    .back-icon
      position absolute
      top 0
      left 0
      font-size .32rem
      color #ffffff
</style>
