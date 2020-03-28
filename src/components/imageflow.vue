<template>
 <div class="imageflow">
    <img src="http://www.choclab.com.cn/choclab-logo.png" class="logo"> 
    <router-view/>
    <Banner/>
    <BottomBanner />
 </div>
</template>

<script>
import Banner from './common/banner';
import BottomBanner from './common/BottomBanner';
export default {
  name: 'ImageFlow',
  components: {
    Banner,
    BottomBanner
  },
  data () {
    return {
      
    }
  }
}
</script>

<style scoped>
.imageflow {
  position: relative;
  min-height: 100%;
  width: 100%;
  background-image: url('http://www.choclab.com.cn/img/bg.jpg');
}
.logo {
  width: 247px;
  position: fixed;
  top: 30px;
  right: 30px;
}
.bottom-banner {
  position: absolute;
  bottom: 0;
}
</style>