<template>
  <div id="app">
    <div class="banner">
      <swiper :options="swiperOption" ref="mySwiper">
        <swiper-slide v-for="items in allData" :key="items">
          <img :src="items" alt="">
        </swiper-slide>
        <div class="swiper-pagination" slot="pagination"></div>
        <div class="swiper-button-prev" slot="button-prev"></div>
        <div class="swiper-button-next" slot="button-next"></div>
        <div class="swiper-scrollbar" slot="scrollbar"></div>
      </swiper>


    </div>
    <router-view/>
  </div>
</template>

<script>
  import Swiper from 'swiper'
export default {
  name: 'App',
  data () {
    return {
      swiperOption: {
        initialSlide:0,
        observer:true,
        observeParents:true,
        paginationClickable: true,
        autoplay : 2000,
        speed: 1000,
        loop:true,
        autoplayDisableOnInteraction : false,
        allowSwipeToNext : true,
        noSwiping : true,
        prevButton : '.swiper-button-prev',
        nextButton : '.swiper-button-next',
        pagination : '.swiper-pagination',
        paginationType : 'bullets',
      },
      allData: [
        '../static/1.webp',
        '../static/2.webp',
        '../static/3.webp',
        '../static/4.webp',
        '../static/5.webp',
        '../static/6.webp',
      ]
    }
  },
  mounted () {

  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
}
  *{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
  }
</style>
