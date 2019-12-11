<template>
  <div class="header">
    <div class="header-left">
      <div class="iconfont iconfont-left">&#xe658;</div>
    </div>
    <div class="header-mid">
      <span class="iconfont">&#xe66b;</span>
      输入城市/景点/游玩主题
    </div>
    <div class="header-right">
      城市
      <span class="iconfont">&#xe659;</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'homeHeader'
}
</script>
<style lang="stylus" scoped>
  @import '~styles/variables.styl'
  .header
    display: flex
    line-height: .86rem
    background: $bgColor
    color: #fff
    // margin-top: 0rem
    .header-left
      width: .64rem
      float: left
      .iconfont-left
        text-align: center
        font-size: .4rem
    .header-mid
      flex: 1
      height: .64rem
      background: #fff
      margin-top: .12rem
      margin-left: .2rem
      border-radius: .1rem
      color: #ccc
      // text-align: center
      line-height: .64rem
      padding-left: .2rem
    .header-right
      width: 1.24rem
      float: right
      text-align: center
</style>
