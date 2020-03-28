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
  name: 'A',
  data () {
    return {
      listImg: []
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
  /*height: 50%;*/
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