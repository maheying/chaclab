<template>
  <div class="water-flow">
    <div class="right-list-image">      
      <div class="waterfall">
        <div class="right-list-image">
          <div v-for="(image, index) in listImg" class="image-box">
            <router-link :to="`/flow/details/${image.Keyword}`">
              <img :src="image.img"  class="image">
            </router-link>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'WaterFlow',
  data () {
    return {
      listImg: [
        {
          Keyword: 'FImage1',
          img: 'http://www.choclab.com.cn/img/2018AW LOOKBOOK/ADIDAS×STELLA MAC/img主图.jpg'
        },
        {
          Keyword: 'FImage2',
          img: 'http://www.choclab.com.cn/img/2018AW LOOKBOOK/BOTH/img主图.png'
        },
        {
          Keyword: 'FImage3',
          img: 'http://www.choclab.com.cn/img/2018AW LOOKBOOK/FIXXIED STUDIOS/img主图.png'
        },
        {
          Keyword: 'FImage4',
          img: 'http://www.choclab.com.cn/img/2018AW LOOKBOOK/KOLOR/img主图.jpg'
        },
        {
          Keyword: 'FImage5',
          img: 'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/AW18 PRONOUNCE in Shanghai/img主图.jpg'
        },
        {
          Keyword: 'FImage6',
          img: 'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/PRONOUNCE 18AW 秀场图/img主图.png'
        },
        {
          Keyword: 'FImage7',
          img: 'http://www.choclab.com.cn/img/2018AW LOOKBOOK/MARNI/img1.jpg'
        },
        {
          Keyword: 'FImage8',
          img: 'http://www.choclab.com.cn/img/2018AW LOOKBOOK/MASION MARGIELA/img1.jpg'
        },
        {
          Keyword: 'FImage9',
          img: 'http://www.choclab.com.cn/img/2018AW LOOKBOOK/POLIQUANT/23.jpg'
        },
        {
          Keyword: 'FImage10',
          img: 'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM01/主图.jpg'
        },
        {
          Keyword: 'FImage11',
          img: 'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM02/主图.jpg'
        },
        {
          Keyword: 'FImage12',
          img: 'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM03/主图.jpg'
        },
        {
          Keyword: 'FImage13',
          img: 'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM04/主图.jpg'
        },
        {
          Keyword: 'FImage14',
          img: 'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM05/主图.jpg'
        },
        {
          Keyword: 'FImage15',
          img: 'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM06/主图.jpg'
        },
        {
          Keyword: 'FImage16',
          img: 'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce01/主图.jpg'
        },
        {
          Keyword: 'FImage17',
          img: 'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce02/主图.jpg'
        },
        {
          Keyword: 'FImage18',
          img: 'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce03/主图.jpg'
        },
        {
          Keyword: 'FImage19',
          img: 'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce04/主图.jpg'
        },
        {
          Keyword: 'CImage1',
          img: 'http://www.choclab.com.cn/img/cuisine/pic-1.jpg'
        },
        
      ]
    }
  },
  mounted () {},
  methods: {}
}
</script>

<style scoped>
.image-box {
  display: inline-block;
}
.waterfall {
  margin-top: 36px;
}
.water-flow {
  margin: 0 auto;
  padding-top: 90px;
  width: 80%;
  max-width: 1280px;
  min-height: auto;
}
.right-list-image {
  width: 100%;
  height: auto;
}

.image {
  margin-top: 20px;
  margin-right: 10px;
  width: 100%;
}
.container{width:80%;margin: 0 auto;}
    /*瀑布流层*/
    .waterfall{
      -moz-column-count:auto; /* Firefox */
      -webkit-column-count:auto; /* Safari 和 Chrome */
      column-count:3;
      -moz-column-gap: 20px;
      -webkit-column-gap: 20px;
      column-gap: 20px;
      -webkit-column-width:auto;
      -moz-column-width:auto;
      column-width:auto;
    }
    /*一个内容层*/
    .item{
      padding: 10px;
      margin: 0 0 10px 0;
      -moz-page-break-inside: avoid;
      -webkit-column-break-inside: avoid;
      break-inside: avoid;
    }
    .item img{
        width: 100%;
        margin-bottom:10px;
    }
</style>