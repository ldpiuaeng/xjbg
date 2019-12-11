<template>
  <div>
    <home-header></home-header>
    <home-swiper></home-swiper>
    <test-slot :options="swiperOption">haha</test-slot>
    <div>test</div>
  </div>
</template>

<script>
import HomeHeader from './components/HomeHeader'
import HomeSwiper from './components/HomeSwiper'
import TestSlot from './components/TestSlot'
export default {
  name: 'home',
  components: {
    HomeHeader,
    HomeSwiper,
    TestSlot
  }
}
</script>
<style></style>
