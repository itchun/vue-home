<template>
  <div>
    <v-navigation></v-navigation>
    <div id="main_home">
      <div id="carousel">
        <slider :pages="pages" :sliderinit="sliderinit"></slider>
      </div>
    </div>
  </div>
</template>

<script>
import Navigation from '@/components/navigation/Navigation.vue'
import slider from 'vue-concise-slider'// 引入slider组件

export default {
  name: 'home',
  el: '#app',
  data () {
    return {
      //图片列表[arr]
      pages: [
        {
          title: '',
          style: {
            background: 'url(src/assets/carousel/1.jpg)'
          }
        },
        {
          title: '',
          style: {
            background: 'url(src/assets/carousel/2.jpg)'
          }
        },
        {
          title: '',
          style: {
            background: 'url(src/assets/carousel/3.jpg)'
          }
        },
        {
          title: 'slide3',
          style: {
            background: '#4bbfc3',
          },
        }
      ],
      //滑动配置[obj]
      sliderinit: {
        currentPage: 0,//当前页码
        thresholdDistance: 500,//滑动判定距离
        thresholdTime: 100,//滑动判定时间
        autoplay: 1000,//自动滚动[ms]
        loop: true,//循环滚动
        direction: 'vertical',//方向设置，垂直滚动
        infinite: 1,//无限滚动前后遍历数
        slidesToScroll: 1,//每次滑动项数
      }
    }
  },
  components: {
    'v-navigation': Navigation,
    'slider': slider
  }
}
</script>

<style>

#main_home {
 /* left: 25%;
  right: 20%;*/
}

</style>
