<template>
  <div class="home">
    <homeheader></homeheader>
    <homeswiper></homeswiper>
    <homeicon></homeicon>
    <!-- 推荐组件 -->
    <recommend></recommend>
    
  </div>
</template>

<script>
// @ is an alias to /src
import homeheader from '@/views/homecomponents/homeheader'
import homeswiper from '@/views/homecomponents/homeswiper'
import homeicon from '@/views/homecomponents/homeicon'
import recommend from '@/views/homecomponents/recommend'
export default {

  name: 'home',
  components: {
    homeheader,
    homeswiper,
    homeicon,
    recommend
    
  }
}
</script>
<style lang="stylus">
   
</style>
