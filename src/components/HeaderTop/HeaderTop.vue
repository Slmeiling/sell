<template>
  <header class="header">
    <slot name="left"></slot>
    <span class="header_title ellipsis">{{title}}</span>
    <slot name="right"></slot>
  </header>
</template>

<script>
export default {
  props:{
    title:String
  }
}
</script>

<style lang="stylus" rel="stylesheet/stylus">
  .header
    width 100%
    height 45px
    display flex
    justify-content center
    align-items center
    background #02a774
    color #fff
    .header_title
      flex 4
      font-size 20px
      text-align center
</style>