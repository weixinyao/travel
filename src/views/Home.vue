<template>
  <div class="home">
    <homeheader></homeheader>
    <homeswiper></homeswiper>
    <homeicon></homeicon>
    <!-- 推荐组件 -->
    <recommend></recommend>
    <!-- 周末组件 -->
    <weekend></weekend>

    
  </div>
</template>

<script>
// @ is an alias to /src
import homeheader from '@/views/homecomponents/homeheader'
import homeswiper from '@/views/homecomponents/homeswiper'
import homeicon from '@/views/homecomponents/homeicon'
import recommend from '@/views/homecomponents/recommend'
import weekend from '@/views/homecomponents/weekend'
export default {

  name: 'home',
  components: {
    homeheader,
    homeswiper,
    homeicon,
    recommend,
    weekend
    
  }
}
</script>
<style lang="stylus">
   
</style>
