<template>
 <div class="banner">
   <div class="letter-box" v-for="(list, index) in letter">
     <div :id="`li${index}`" :class="['banner-letter', {'underline':index == active}]" @click="letterClick(index)">{{list.name}}</div>
   </div>
 </div>
</template>

<script>
export default {
  name: 'Banner',
  data () {
    return {
      active: 0,
      letter: [
        {
          name: 'N',
          decoration: false
        },
        {
          name: 'F',
          decoration: false
        },
        {
          name: 'A',
          decoration: false
        },
        {
          name: 'C',
          decoration: false
        },
        {
          name: 'M',
          decoration: false
        }
      ]
    }
  },
  mounted () {},
  methods: {
    letterClick(index) {
    this.active = index;
    if(index === 1) {
      this.$router.push('/flow/Fpage');
    } else if( index === 2) {
      this.$router.push('/flow/Apage');
    } else if(index === 3) {
      this.$router.push('/flow/Cpage');
    }else if(index === 4){
      this.$router.push('/flow/map');
    } else {
      this.$router.push('/flow');
    }
    }
  }
}
</script>

<style scoped>
@font-face {
  font-family: 'BEBAS__'
}
.banner {
  z-index: 999;
  width: 72px;
  height: 580px;
  display: inline-block;
  position: fixed;
  top: 0; 
  background: #182f79;
}
.letter-box {
  height: 20%;
  width: 100%;
  line-height: 116px;
}
.banner-letter {
  text-align: center;
  color: #fff;
  font-size: 50px;
  font-weight: 700;
  font-family: 'BEBAS'
}
.underline {
  text-decoration:underline;
}
</style>