<template>
 <div class="picdetail">
   <div>
     <img :src="imgArray" v-for="imgArray in showList.li" class="liImg">
    <p class="item-text">{{showList.text}}</p>
   </div>
 </div>
</template>
<script>
  export default {
    name: 'Picdetail',
    data() {
      return {
        showList: '',
        list: [
          {
            id: 'FImage1',
            li: [
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/ADIDAS×STELLA MAC/img主图.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/ADIDAS×STELLA MAC/图片1.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/ADIDAS×STELLA MAC/图片6.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/ADIDAS×STELLA MAC/图片7.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/ADIDAS×STELLA MAC/图片8.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/ADIDAS×STELLA MAC/图片13.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/ADIDAS×STELLA MAC/图片14.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/ADIDAS×STELLA MAC/图片17.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/ADIDAS×STELLA MAC/图片18.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/ADIDAS×STELLA MAC/图片19.jpg'
            ]
          },
          {
            id: 'FImage2',
            li: [
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/BOTH/img主图.png',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/BOTH/img1.png',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/BOTH/img6.png',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/BOTH/img7.png',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/BOTH/img8.png',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/BOTH/img9.png',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/BOTH/img10.png',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/BOTH/img11.png',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/BOTH/img12.png',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/BOTH/img13.png',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/BOTH/img21.png',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/BOTH/img23.png',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/BOTH/img26.png',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/BOTH/img27.png'
            ]
          },
          {
            id: 'FImage3',
            li: [
             'http://www.choclab.com.cn/img/2018AW LOOKBOOK/FIXXIED STUDIOS/img主图.png',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/FIXXIED STUDIOS/img1.png',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/FIXXIED STUDIOS/img2.png',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/FIXXIED STUDIOS/img3.png',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/FIXXIED STUDIOS/img4.png',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/FIXXIED STUDIOS/img5.png',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/FIXXIED STUDIOS/img6.png',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/FIXXIED STUDIOS/img7.png',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/FIXXIED STUDIOS/img8.png',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/FIXXIED STUDIOS/img9.png',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/FIXXIED STUDIOS/img10.png',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/FIXXIED STUDIOS/img11.png',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/FIXXIED STUDIOS/img12.png',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/FIXXIED STUDIOS/img13.png',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/FIXXIED STUDIOS/img14.png'
            ]
          },
          {
            id: 'FImage4',
            li: [
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/KOLOR/img主图.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/KOLOR/img1.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/KOLOR/img2.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/KOLOR/img3.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/KOLOR/img4.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/KOLOR/img5.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/KOLOR/img6.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/KOLOR/img7.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/KOLOR/img8.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/KOLOR/img9.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/KOLOR/img10.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/KOLOR/img11.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/KOLOR/img12.jpg'
            ]
          },
          {
            id: 'FImage5',
            li: [
             'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/AW18 PRONOUNCE in Shanghai/img主图.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/AW18 PRONOUNCE in Shanghai/img1.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/AW18 PRONOUNCE in Shanghai/img2.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/AW18 PRONOUNCE in Shanghai/img3.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/AW18 PRONOUNCE in Shanghai/img4.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/AW18 PRONOUNCE in Shanghai/img5.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/AW18 PRONOUNCE in Shanghai/img6.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/AW18 PRONOUNCE in Shanghai/img7.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/AW18 PRONOUNCE in Shanghai/img8.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/AW18 PRONOUNCE in Shanghai/img9.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/AW18 PRONOUNCE in Shanghai/img10.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/AW18 PRONOUNCE in Shanghai/img11.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/AW18 PRONOUNCE in Shanghai/img12.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/AW18 PRONOUNCE in Shanghai/img13.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/AW18 PRONOUNCE in Shanghai/img14.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/AW18 PRONOUNCE in Shanghai/img15.jpg',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/AW18 PRONOUNCE in Shanghai/img16.jpg'
            ]
          },
          {
            id: 'FImage6',
            li: [
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/PRONOUNCE 18AW 秀场图/img主图.png',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/PRONOUNCE 18AW 秀场图/img1.png',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/PRONOUNCE 18AW 秀场图/img2.png',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/PRONOUNCE 18AW 秀场图/img3.png',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/PRONOUNCE 18AW 秀场图/img4.png',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/PRONOUNCE 18AW 秀场图/img5.png',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/PRONOUNCE 18AW 秀场图/img6.png',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/PRONOUNCE 18AW 秀场图/img7.png',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/PRONOUNCE 18AW 秀场图/img8.png',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/PRONOUNCE 18AW 秀场图/img9.png',
            'http://www.choclab.com.cn/img/2018AW LOOKBOOK/PRONOUNCE/PRONOUNCE 18AW 秀场图/img10.png'
            ]
          },
          {
            id: 'FImage7',
            li: [
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/MARNI/img1.jpg',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/MARNI/img2.jpg',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/MARNI/img3.jpg'
            ]
          },
          {
            id: 'FImage8',
            li: [
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/MASION MARGIELA/img1.jpg',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/MASION MARGIELA/img2.jpg',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/MASION MARGIELA/img3.jpg',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/MASION MARGIELA/img4.jpg',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/MASION MARGIELA/img5.jpg',
            ]
          },
          {
            id: 'FImage9',
            li: [
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/POLIQUANT/23.jpg',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/POLIQUANT/01.jpg',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/POLIQUANT/02.jpg',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/POLIQUANT/03.jpg',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/POLIQUANT/04.jpg',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/POLIQUANT/05.jpg',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/POLIQUANT/06.jpg',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/POLIQUANT/07.jpg',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/POLIQUANT/08.jpg',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/POLIQUANT/09.jpg',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/POLIQUANT/10.jpg',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/POLIQUANT/11.jpg',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/POLIQUANT/12.jpg',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/POLIQUANT/13.jpg',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/POLIQUANT14.jpg',
              'http://www.choclab.com.cn/img/2018AW LOOKBOOK/POLIQUANT/15.jpg'
            ] 
          },
          {
            id: 'FImage10',
            li: [
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM01/主图.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM01/01.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM01/02.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM01/03.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM01/04.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM01/05.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM01/06.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM01/07.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM01/08.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM01/09.jpg'
            ]
          },
          {
            id: 'FImage11',
            li: [
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM02/主图.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM02/01.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM02/02.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM02/03.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM02/04.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM02/05.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM02/06.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM02/07.jpg'
            ]
          },
          {
            id: 'FImage12',
            li: [
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM03/主图.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM03/01.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM03/02.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM03/03.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM03/04.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM03/05.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM03/06.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM03/07.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM03/08.jpg'
            ]
          },
          {
            id: 'FImage13',
            li: [
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM04/主图.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM04/01.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM04/02.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM04/03.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM04/04.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM04/05.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM04/06.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM04/07.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM04/08.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM04/09.jpg'
            ]
          },
          {
            id: 'FImage14',
            li: [
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM05/主图.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM05/01.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM05/02.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM05/03.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM05/04.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM05/05.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM05/06.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM05/07.jpg'
            ]
          },
          {
            id: 'FImage15',
            li: [
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM06/主图.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM06/01.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM06/02.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM06/03.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM06/04.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM06/05.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM06/06.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM06/07.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM06/08.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/MSGM06/09.jpg'
            ]
          },
          {
            id: 'FImage16',
            li: [
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce01/主图.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce01/01.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce01/02.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce01/03.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce01/04.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce01/05.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce01/06.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce01/07.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce01/08.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce01/09.jpg'
            ]
          },
          {
            id: 'FImage17',
            li: [
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce02/主图.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce02/01.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce02/02.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce02/03.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce02/04.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce02/05.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce02/06.jpg'
            ]
          },
          {
            id: 'FImage18',
            li: [
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce03/主图.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce03/01.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce03/02.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce03/03.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce03/04.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce03/05.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce03/06.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce03/07.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce03/08.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce03/09.jpg'
            ]
          },
          {
            id: 'FImage19',
            li: [
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce04/主图.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce04/01.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce04/02.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce04/03.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce04/04.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce04/05.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce04/06.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce04/07.jpg',
              'http://www.choclab.com.cn/img/2018AW%20LOOKBOOK/Pronounce04/08.jpg'
            ]
          },
          {
            id: 'CImage1',
            li: [
              'http://www.choclab.com.cn/img/cuisine/pic-1.jpg',
              'http://www.choclab.com.cn/img/cuisine/pic-2.jpg',
              'http://www.choclab.com.cn/img/cuisine/pic-3.jpg',
              'http://www.choclab.com.cn/img/cuisine/pic-4.jpg'
            ]
          }
        ]
      }
    },
    beforeMount() {
      this.list.forEach((item) => {
        if(item.id == this.$route.params.id) {
          this.showList = item;
        }
      })
    }
  }
</script>

<style scoped>
.picdetail {
  width: 70%;
  max-width: 1024px;
  height: auto;
  margin: 0 auto;
  padding-top: 134px;
}
.liImg {
  margin: auto;
  display: block;
  margin-top: 10px;
  width: 100%;
}
.item-text {
  width: 50%;
  margin: auto;
  text-align: center;
  display: block;
  color: #000;
  font-size: 20px;
  margin-top: 50px;
}
</style>