<template>
    <div class="header">
        <div class="header-left"><div class="iconfont back-icon">&#xe624;</div></div>
        <div class="header-input"><span class="iconfont">&#xe632;</span>输入城市/景点/游玩主题</div>
        <div class="header-right">{{this.city}}<span class="iconfont arrow-icon">&#xe6aa;</span></div>
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

<style lang="stylus" scoped>
    .header
        display:flex
        line-height:.86rem
        color:#fff
        background:#00bcd4
        .header-left
            width:.64rem
            float:left
            .back-icon
                text-align:center
                font-size:.4rem
        .header-input
            flex:1
            height:.64rem
            line-height:.64rem
            margin-top:.12rem
            margin-left:.2rem
            padding-left:.2rem
            background:#fff
            border-radius:.1rem
            color:#ccc
        .header-right
            width:1.24rem
            float:right
            text-align:center
            .arrow-icon
                font-size.24rem
</style>
