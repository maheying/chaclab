<template>
  <div>
  <div class="index-page">
    <router-link to="flow">
      <div class="index-page-img">
        <img src="http://www.choclab.com.cn/img/choclab-1.jpg">
      </div>
    </router-link>
  </div>
  <BottomBanner />
</div>
</template>

<script>
import BottomBanner from './common/BottomBanner';
export default {
  name: 'Index',
  components: {
    BottomBanner,
  },
  data() {
    return{
    }
  },
  computed: {
    
  },
  methods: {
   
  }
}
</script>

<style>
.index-page {
  overflow: hidden;
  width: 100%;
  height: 100%;
  -webkit-display:flex;
  display:flex;
  -webkit-align-items:center;
  align-items:center;
}
a {
  display: block;
  width: 100%;
}
.index-page-img img{
  width: 100%;
}
.bottom-banner {
  width: 100%;
  height: 20px;
  background: #fafafa;
  color: #bbbbbb;
  text-align: right;
  font-size: 12px;
  line-height: 20px;
  position: fixed;
  bottom: 0;
}
</style>