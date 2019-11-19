<template>
<div class="wrapper">
   <swiper :options="swiperOption">
    <!-- slides -->
    <swiper-slide v-for="item in swiperlist" :key="item.id">
        <img class="swiperimage" :src=item.imgUrl alt="">
    </swiper-slide>
    <!-- Optional controls -->
    <div class="swiper-pagination"  slot="pagination"></div>
  </swiper>
</div> 
</template>
<script>
export default {
    name: 'homeswiper',
    data() {
        return {
          swiperOption: {
                // 参数选项,显示小点
                pagination: { el: ".swiper-pagination" },
                loop: true
        },
        swiperlist: [
        {
            id: 1,
            imgUrl: '//imgcps.jd.com/ling4/2669346/5L-d5rip5p2v5aSn54mM5q2j5ZOB/5ruh5oSP6LSt5Lqs5Zac/p-5c13515d82acdd181dcbdc35/d7fc40a0/cr_1125x445_0_171/s1125x690/q70.jpg'
        },
        {
            id: 2,
            imgUrl: '//m.360buyimg.com/mobilecms/s700x280_jfs/t1/72441/34/15136/284783/5dcd4da0E30297ede/5c94bfdc635405f3.jpg!cr_1125x445_0_171!q70.jpg.dpg'

        },
        {
            id: 3,
            imgUrl: '//m.360buyimg.com/mobilecms/s700x280_jfs/t1/86804/31/2230/127552/5dccf247E6d9ca7a8/a153475e8ef3ab4b.jpg!cr_1125x445_0_171!q70.jpg.dpg'
        }
        ]
    }
    }
    
}
</script>
<style lang="stylus" scoped>
.wrapper
  width: 100%
  height: 0
  padding-bottom: 31.25%
  overflow: hidden
  .swiperimage
    width: 100%
</style>