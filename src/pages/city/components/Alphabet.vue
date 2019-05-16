<template>
  <ul class="list">
    <li class="item" v-for="(item, key) of list" :key="key">{{key}}</li>
  </ul>
</template>

<script>
export default {
  name: 'cityAlphabet',
  props: {
    list: Object
  }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/varibles.styl'
  .list
    position absolute
    display flex
    flex-direction column
    justify-content center
    right 0
    top 1.58rem
    bottom 0
    width .4rem
    .item
      line-height .4rem
      text-align center
      color $bgColor
</style>
