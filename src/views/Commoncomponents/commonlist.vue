<template>
  <div class="goods">
    <div class="hot">
       <div class="title">热门搜索</div>
       <ul class="buttonlist">
        <router-link to="/">
           <li>高等数学</li>
        </router-link>
           <li>条纹衬衫</li>
           <li>502胶水</li>
           <li>线性代数</li>
           <li>口红</li>
       </ul>
    </div>
    <div class="goodlist" ref="wrapper">
        <div class="content">
            <router-link to="/">
            <div class="good">
              <div class="pic">
                <img src="//imgs.qunarzz.com/p/tts8/1607/59/e5e56c66a90e599a.jpg_r_480x320x90_dd143fb3.jpg" alt="">
              </div>
                <span class="font">高等数学</span>
            </div>
            </router-link>
            <router-link to="/">
            <div class="good">
              <div class="pic">
                <img src="//imgs.qunarzz.com/p/tts8/1607/59/e5e56c66a90e599a.jpg_r_480x320x90_dd143fb3.jpg" alt="">
              </div>
                <span class="font">高等数学</span>
            </div>
            </router-link>
            <router-link to="/">
            <div class="good">
              <div class="pic">
                <img src="//imgs.qunarzz.com/p/tts8/1607/59/e5e56c66a90e599a.jpg_r_480x320x90_dd143fb3.jpg" alt="">
              </div>
                <span class="font">高等数学</span>
            </div>
            </router-link>
            <router-link to="/">
            <div class="good">
              <div class="pic">
                <img src="//imgs.qunarzz.com/p/tts8/1607/59/e5e56c66a90e599a.jpg_r_480x320x90_dd143fb3.jpg" alt="">
              </div>
                <span class="font">高等数学</span>
            </div>
            </router-link>
            <router-link to="/">
            <div class="good">
              <div class="pic">
                <img src="//imgs.qunarzz.com/p/tts8/1607/59/e5e56c66a90e599a.jpg_r_480x320x90_dd143fb3.jpg" alt="">
              </div>
                <span class="font">高等数学</span>
            </div>
            </router-link>
            <router-link to="/">
            <div class="good">
              <div class="pic">
                <img src="//imgs.qunarzz.com/p/tts8/1607/59/e5e56c66a90e599a.jpg_r_480x320x90_dd143fb3.jpg" alt="">
              </div>
                <span class="font">高等数学</span>
            </div>
            </router-link>
      </div>
    </div>
  </div>
</template>
<script>
import BScroll from 'better-scroll'
export default {
    name: 'commonlist',
    mounted() {
       this.scroll = new BScroll(this.$refs.wrapper)
    }

}
</script>
<style lang="stylus" scoped>
.hot
  height: 3.4rem
  border-bottom: .03rem solid pink
  .title
    font-size: .32rem
    text-indent: .1rem
    width: 100%
    height: .86rem
    line-height: .86rem
    background-color: pink 
    color: #fff
    margin-bottom: .01rem
    margin-top: .05rem
  .buttonlist
    li
      color: red
      border: .1rem solid pink 
      height: .84rem
      line-height: .84rem
      width: 1.9rem
      float: left 
      border-radius: .4rem
      margin: .09rem .1rem
      text-align:center
.goodlist  
  height: 8rem
  overflow: hidden
.goodlist .content 
  overflow: hidden
.goodlist .content .good
  margin-left: .4rem
  margin-top: .4rem
  border: .1rem solid pink
  width: 3.1rem
  height: 3.1rem
  padding-top: .1rem
  padding-left: .2rem
  box-sizing:border-box
  float: left
.goodlist .content .good .font
  text-align: center
  color: #666
  width: 2.5rem
  display:inline-block
  margin-top: .05rem
.goodlist .content .good .pic img
   width: 2.5rem
   height: 2.5rem
   
</style>