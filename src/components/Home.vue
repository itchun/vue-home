<template>
  <div>
    <v-navigation></v-navigation>
    <div id="main_home">
      <div id="carousel">
        <slide-show :slides="slides"></slide-show>
      </div>
    </div>
  </div>
</template>

<script>
import Navigation from '@/components/navigation/Navigation.vue'
import slideShow from '@/components/utils/slideShow.vue'

export default {
  name: 'home',
  data () {
    return {
      slides: [
        {
          src: require('../assets/carousel/1.jpg'),
          title: '',
        },
        {
          src: require('../assets/carousel/2.jpg'),
          title: '',
        },
        {
          src: require('../assets/carousel/3.jpg'),
          title: '',
        }
      ]
    }
  },
  components: {
    'v-navigation': Navigation,
    'slide-show': slideShow
  }
}
</script>

<style>

#carousel {



}

</style>
