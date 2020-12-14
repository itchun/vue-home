<template>
  <div id="navigation">
    <div class="navigation_inner">
      <a class="logo_info" href="">{{ logo_info }}</a>
      <div class="home_div">
        <a class="home 1" href="">{{ home_1 }}</a>
        <a class="home 2" href="">{{ home_2 }}</a>
        <a class="home 3" href="">{{ home_3 }}</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Navigation',
  data () {
    return {
      logo_info: '李淑玲',
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
  background-color: #333333;
  background-repeat: no-repeat;
  background-size: 100% 100%;
  height: 45px;
}

.navigation_inner {
  position: absolute;
  left: 17%;
  right: 20%;
  font-family: 'Microsoft Himalaya';
  height: 30px;
  top: 5px;
}

.logo_info {
  float: left;
  font-size: 26px;
  width: 3.14286em;
}

.home_div {

}

.home {
  float: right;
  font-size: 20px;
  margin-right: 100px;
  margin-top: 3px;
}

a {
  text-decoration: none;
  color: #eaeaea;
}
</style>
