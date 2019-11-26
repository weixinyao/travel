<template>
    <div>
        <!--搜索标题 -->
        <commonheader></commonheader>
        <!-- 搜索框 -->
        <commonsearch></commonsearch>
        <!-- 热搜 -->
        <commonlist></commonlist>
    </div>
</template>
<script>
import commonheader from '@/views/Commoncomponents/commonheader'
import commonsearch from '@/views/Commoncomponents/commonsearch'
import commonlist from '@/views/Commoncomponents/commonlist'
export default {
    name: 'Common',
    components: {
        commonheader,
        commonsearch,
        commonlist
    }
}
</script>
<style lang="stylus" scoped>

</style>