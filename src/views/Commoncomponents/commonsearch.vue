<template>
   <div class="search">
    <input class="searchinput" type="text" placeholder="请输入商品名称" />
   </div>
</template>
<script>
export default {
    name: 'commonsearch'
}
</script>
<style lang="stylus" scoped>
  .search
    height: .86rem
    line-height: .86rem
    padding: 0 .2rem
    background-color: pink
    .searchinput
      width: 100%
      height: .74rem
      border: .01rem dotted orange
      border-radius: .1rem
      text-align: center
</style>