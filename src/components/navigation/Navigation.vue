<template>
  <div id="navigation">
    <div class="navigation_inner">
      <a class="logo_info" href="">{{ logo_info }}</a>
      <a class="home 1" href="">{{ home_1 }}</a>
      <a class="home 2" href="">{{ home_2 }}</a>
      <a class="home 3" href="">{{ home_3 }}</a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Navigation',
  data () {
    return {
      logo_info: '王春的个人网站',
      home_1: '主页',
      home_2: '博客',
      home_3: '留言板'
    }
  }
}

</script>

<style>

* {
  margin: 0;
  padding: 0;
}

#navigation {
  background-image: url("../../assets/navigation/backImage.png");
  background-repeat: no-repeat;
  background-size: 100% 100%;
  height: 100px;
}

.navigation_inner {
  position: absolute;
  top: 20px;
  left: 25%;
  right: 20%;
  font-family: 'Microsoft Himalaya';
}

.logo_info{
  font-size: 40px;
}

.home{
  font-size: 30px;
  margin: 55px;
}

a{
  text-decoration: none;
  color: #000000;
}
</style>
