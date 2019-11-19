<template>
  <div class="header">
    <div class="headerleft">
      <div class="iconfont backicon">&#xe624;</div>
    </div>
    <div class="headercenter">
      <span class="iconfont">&#xe632;</span>
      输入城市/景点/游玩主题</div>
    <div class="headerright">
      城市
      <span class="iconfont arrowicon">&#xe64a;</span>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'homeheader',
  components: {
    
  }
}
</script>
<style lang="stylus" scoped>
@import '~@/assets/style/globalvaribles.styl'
  .header
    line-height: .86rem
    display: flex
    background-color: $bgcolor
    .headerleft
      width: .64rem
      float: left
      .backicon
        text-align: center
        font-size: .4rem
        color: #fff
    .headerright
      width: 1.24rem
      float: right
      text-align: center
      color: #fff
      .arrowicon
        font-size: .24rem
        margin-left: -.04rem
        color: #fff
    .headercenter
      color: #ccc
      height: .64rem
      line-height: .64rem
      flex: 1
      background-color: #fff
      border-radius: .1rem
      margin-top: .12rem
      margin-left: .2rem
      padding-left: .2rem
</style>
