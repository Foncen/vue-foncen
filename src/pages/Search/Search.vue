<template>
  <div>
    <section class="search">
      <HeaderTop title="搜索"/>
      <form class="search_form" action="#">
        <input type="search" name="search" placeholder="请输入商家或美食名称" class="search_input">
        <input type="submit" name="search" value="搜索" class="search_submit">
      </form>
    </section>
  </div>
</template>

<script>
  import HeaderTop from '../../components/HeaderTop/HeaderTop'

  export default {
    name: 'FooterGuide',
    components: {
      HeaderTop
    }
  }
</script>

<style lang="stylus" rel="stylesheet/stylus">

  .search
    overflow hidden
    .search_form
      clearFix()
      margin-top 45px
      background-color #fbfff0
      padding 12px 8px

      input
        height 35px
        padding 0 4px
        border-radius 2px
        font-weight bold
        outline none

        &.search_input
          float left
          width 79%
          border 4px solid #87c9f2
          font-size 14px
          color #333
          background-color #f2de77

        &.search_submit
          float right
          width 18%
          border 4px solid #e1eff4
          font-size 16px
          color #44eeff
          background-color #090406
</style>
