<template>
    <div class="wrapper">
        <swiper :options="swiperOption" ref="mySwiper" @someSwiperEvent="callback">
    <swiper-slide v-for="item of swiperList" :key="item.id">
        <img class="swiper-img" :src="item.ingUrl"/>
    </swiper-slide>
    <div class="swiper-pagination"  slot="pagination"></div>
  </swiper>
    </div>
</template>

<script>
export default {
    name: 'HomeSwiper',
    data () {
        return {
            swiperOption: {
                pagination: '.swiper-pagination',
                loop: true
            },
            swiperList: [{
                id: '0001',
                ingUrl: 'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20195/dc11f0bb94057224b104a2017f313e21.jpg_750x200_feee379d.jpg'
            },{
                id: '0002',
                ingUrl: 'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20194/522b43cda83d29460da14ec8975b4060.jpg_750x200_2ff9e60a.jpg'
            }]
        }
    }
}
</script>

<style lang="stylus" scoped>
.wrapper >>> .swiper-pagination-bullet-active
    background : #fff
.wrapper
    overflow: hidden
    width: 100%
    height: 0
    padding-bottom: 26.7%
    background: #ddd
    .swiper-img
        width: 100%
</style>
