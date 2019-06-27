<template>
  <!--头部-->
    <header class="header">
        <slot name="left"></slot> <!-- 插槽元素-->
        <span class="header_title">
            <span class="header_title_text ellipsis">{{title}}</span>
        </span>
        <slot name="right"></slot> <!-- 插槽元素-->
    </header>
</template>

<script>
export default {
  data () {
    return {
    }
  },
  props: {
      title: String
  }
}
</script>

<style lang="stylus" rel="stylesheet/stylus" scoped>
.header
    background-color #02a774
    position fixed
    top 0
    left 0
    width 100%
    height 45px
    .header_search
        float left
        line-height 45px
        height 45px
        width 10%
        margin-left 5px
        display inline-block
        .icon-sousuo
            font-size 25px
            color #fff
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
        display inline-block
        float right
        margin-right 5px
        text-align center
        font-size 14px
        color #fff
        width 70px
        line-height 45px
        height 45px
        .header_login_text
            color #fff
</style>