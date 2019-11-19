<template>
  <div class="recommend">
      <div class="recommendtitle">周末去哪儿</div>
      <ul>
          <li class="item" v-for="item in travelList" :key="item.id">
              <div class="item-img-wrapper">
                  <img class="itemimg" :src="item.imgUrl" alt="">
              </div>
              <div class="iteminfo">
                  <p class="itemtitle">
                        {{item.title}}
                  </p>
                  <p class="itemdesc">
                      {{item.desc}}
                  </p>
              </div>
          </li>
      </ul>
  </div>
</template>
<script>
export default {
    name: 'weekend',
    data() {
      return {
        travelList: [
          {
            id: '001',
            imgUrl: '//imgs.qunarzz.com/p/tts6/1805/2b/254b1e79fae33302.jpg_r_390x260x90_06d7d6c3.jpg',
            title: '深圳-香港 3天跟团游',
            desc: '双11立减活动深圳往返！经典纯玩游！港珠澳大桥！港澳3日！观光+自由行+澳门'
          },
          {
            id: '002',
            imgUrl: '//imgs.qunarzz.com/vs_ceph_vs_tts/5958b155-6345-4dc8-afea-881a83d90c60.jpg_r_480x320x90_c9422665.jpg',
            title: '深圳-海口 5天跟团游',
            desc: '三亚超值纯玩派5日游+帆船游艇出海！分界洲/大小洞天/天涯海角/亚龙湾玫瑰谷'
          },
          {
            id: '003',
            imgUrl: '//imgs.qunarzz.com/vs_ceph_vs_tts/67d500ae-a5c7-42a8-9ca8-2be5da8ba921.jpg_r_480x320x90_4c6597bf.jpg',
            title: '深圳-桂林 4天跟团游',
            desc: '错峰金秋游桂林龙脊古东瀑布丨民族自助宴+遇龙河双人漂流丨漓江阳朔银子岩'
          },
          {
            id: '004',
            imgUrl: '//imgs.qunarzz.com/p/tts8/1703/e2/149f578bbb9c7302.jpg_r_480x320x90_0df92e9d.jpg',
            title: '深圳-桂林 3天跟团游',
            desc: '漓悠悠纯玩！蝴蝶泉侗王夜宴+遇龙河竹筏+象鼻山银子岩+漓江游船/桂林阳朔3日'
          }
        ]
      }
    }
}
</script>
<style lang="stylus" scoped>

  .recommendtitle
    line-height: .8rem
    background-color: #eee
    margin-top: .2rem
    text-indent: .2rem
  .item-img-wrapper
    overflow: hidden
    .itemimg
      width: 100%
      padding: .1rem
  .iteminfo
    min-width: 0
    padding: .1rem
    .itemtitle
      font-size: .32rem 
      line-height: .54rem
      overflow: hidden
      white-space: nowrap 
      text-overflow: ellipsis
    .itemdesc
      color: blue
      line-height: .4rem
      color: #ccc
      overflow: hidden
      white-space: nowrap 
      text-overflow: ellipsis
</style>