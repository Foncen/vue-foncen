<template>
  <header class="header">
    <slot name="left"></slot>
    <a class="header_title">
      <span class="header_title_text ellipsis">{{title}}</span>
    </a>
    <slot name="right"></slot>
  </header>
</template>
<div>

</div>
<script>
  export default {
    name: 'HeaderTop',
    props:{
      title: String
    }
  }
</script>

<style lang="stylus" rel="stylesheet/stylus">

  @import "../../common/stylus/mixin.styl"
  .header
    background-color #090406
    position fixed
    z-index 205
    left 0
    top 0
    width 100%
    height 45px

    .header_search
      position absolute
      left 15px
      top 50%
      transform translateY(-50%)
      width 10%
      height 50%

      .icon-chaxun
        font-size 25px
        color #ff2126

    .header_title
      position absolute
      top 50%
      left 50%
      transform translate(-50%, -50%)
      width 50%
      color #fff
      text-align center

      .header_title_text
        font-size 20px
        color #fff
        display block

    .header_login
      font-size 14px
      color #fff
      position absolute
      right 15px
      top 50%
      transform translateY(-50%)

      .header_login_text
        color #fff

</style>
