
<template>
 <div class='mapWrapper'>
    <!--<img class='mapImage' src="http://www.choclab.com.cn/img/store/map-position.jpg">-->
     <div class='mapFlow'>
       <div v-for="(image, index) in imgList" 
        :class="['mapBox', {'rightZero': (index+1) % 3 == 0}]">
          <MapFlowList :data="image" />
       </div>
     </div>
 </div>
</template>

<style type="text/css" scoped>
  .mapWrapper{
    width: 1280px;
    margin: 0 auto;
    padding: 0 20px;
  }
 .mapImage {
    width: 100%;
    margin-bottom: 20px;
  }
  .mapFlow{
    padding-top: 145px;
  }
  .mapFlow:after{
    content:".";
    clear:both;
    display:block;
    height:0;
    overflow:hidden;
    visibility:hidden;
  }
  .mapBox{
    float:left;
    width: 400px;
    height: 420px;
    margin-bottom: 20px;
    margin-right: 20px;
  }
  @media screen and (max-width: 1190px){
    .mapWrapper{
      width: 990px;
      margin: 0 auto;
      padding: 0;
    }
    .mapBox{
      width: 326px;
      height: 330px;
      margin-bottom: 6px;
      margin-right: 6px;
    }
    .mapImage {
      height: 556px;
    }
  }
  .rightZero {
    margin-right: 0;
  }
</style>
<script>
import MapFlowList from './mapflowList'
import dataInit from '../../assets/imgdata.js'
export default {
  name: 'MapFlow',
  data () {
    return {
      imgList: dataInit.mapImg
    }
  },
  computed: {
    
  },
  components: {
    MapFlowList
  },
  methods:{

  }
}
</script>