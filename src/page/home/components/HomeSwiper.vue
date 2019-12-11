<template>
  <md-card>
    <md-card-media>
      <!-- swiper -->
      <div class="wrapper">
      <swiper :options="swiperOption">
      <!-- slides -->
        <swiper-slide v-for='item in swiperList' :key="item.id">
          <img class = 'swiper-img' :src='item.imgUrl'/>
        </swiper-slide>
      <!-- Optional controls -->
        <div class="swiper-pagination"  slot="pagination"></div>
        </swiper>
      </div>
    </md-card-media>
  </md-card>
</template>

<script>
export default {
  name: 'HomeSwiper',
  data () {
    return {
      swiperOption: {
        pagination: {
          el: '.swiper-pagination',
          dynamicBullets: true
        },
        loop: true
      },
      swiperList: [{
        id: '001',
        imgUrl: '//imgs.qunarzz.com/vc/aa/9e/82/14bf523635542806a671763e98.jpg_92.jpg'
      }, {
        id: '002',
        imgUrl: '//imgs.qunarzz.com/vc/44/e9/86/95bc36c9e1c06ebd68bdfe222e.jpg_92.jpg'
      }, {
        id: '003',
        imgUrl: '//mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20198/b59b8db9f72eb8f54df5bf2155672e9c.jpg'
      }, {
        id: '004',
        imgUrl: '//imgs.qunarzz.com/vc/aa/9e/82/14bf523635542806a671763e98.jpg_92.jpg'
      }
      ]
    }
  }
  // computed: {
  //   swiper () {
  //     return this.$refs.mySwiper.swiper
  //   }
  // },
  // mounted () {
  //   // current swiper instance
  //   // 然后你就可以使用当前上下文内的swiper对象去做你想做的事了
  //   console.log('this is current swiper instance object', this.swiper)
  //   this.swiper.slideTo(3, 1000, true)
  // }
}
</script>
<style lang='stylus' scoped>
  .wrapper
    width: 100%
    height: 0
    overflow: hidden
    padding-bottom: 31.25%
    background: #eee
    .swiper-img
      width: 100%
</style>
