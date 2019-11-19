<template>
    <div class="imageicon">
     <swiper :options="swiperOption">
        <swiper-slide v-for="(page,index) in pages" :key="index">
        <div class="icon" v-for="item in page" :key="item.id">
            <div class="iconimage"> 
            <img :src="item.imgUrl" alt="">
            </div>
            <p>{{item.desc}}</p>
        </div>
        </swiper-slide>
    </swiper>
    </div>
</template>
<script>
export default {
    name: 'homeicon',
    data() {
        return {
            iconlist: [
                {
                   
                       id: '001',
                       imgUrl: '//s.qunarzz.com/homenode/images/touchheader/hotel.png',
                       desc: '酒店'
                   
                },
                {
                      id: '002',
                      imgUrl: '//s.qunarzz.com/homenode/images/touchheader/flight.png',
                      desc: '机票'
                },
                {
                    id: '003',
                    imgUrl: '//s.qunarzz.com/homenode/images/touchheader/package.png',
                    desc: '度假'
                },
                {
                    id: '004',
                    imgUrl: '//s.qunarzz.com/homenode/images/touchheader/train.png',
                    desc: '火车票'
                },
                {
                    id: '005',
                    imgUrl: '//s.qunarzz.com/homenode/images/touchheader/piao.png',
                    desc: '景点门票'
                },
                {
                    id: '006',
                    imgUrl: "//s.qunarzz.com/homenode/images/touchheader/innBnb.png",
                    desc: '民宿客栈'
                },
                {
                    id: '007',
                    imgUrl: '//s.qunarzz.com/homenode/images/touchheader/bargainflight.png',
                    desc: '低价机票'
                },
                {
                    id: '008',
                    imgUrl: '//s.qunarzz.com/homenode/images/touchheader/group.png',
                    desc: '特惠酒店'
                },
                {
                    id: '009',
                    imgUrl: '//s.qunarzz.com/homenode/images/touchheader/haiwai.png',
                    desc: '海外酒店'
                }
            ],
            swiperOption: {
                autoplay: false
            }
        }
    },
    computed: {
        pages() {
            const pages = []
            this.iconlist.forEach((item,i) => {
              let index = Math.floor(i/8)
                if(!pages[index]) {
                    pages[index] = []
                }
                pages[index].push(item)
                
            });
            return pages
        }
    }
}
</script>
<style lang="stylus" scoped>
  .imageicon >>> .swiper-container
    width: 100%
    height: 0
    padding-bottom: 50%
    overflow: hidden
    .icon
      width: 25%
      height: 0
      text-align: center
      padding-bottom: 25%
      overflow: hidden
      float: left 
      .iconimage
        margin-top: .2rem
        margin-bottom: .2rem
      .iconimage img
        width: 50%
        height: 50%

      
      
        
        
        
      
</style>