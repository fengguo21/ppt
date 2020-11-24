<template>
  <div class="dashboard">

    <div class="jumbotron">
      <h1 class="display-4">条形码</h1>
      <p class="lead">条形码(barcode)是将宽度不等的多个黑条和空白，按照一定的编码规则排列，用以表达一组信息的图形标识符。常见的条形码是由反射率相差很大的黑条（简称条）和白条（简称空）排成的平行线图案。</p>
      <hr class="my-4">
      <img src="../../assets/imgs/oneDemo.jpeg" class="bigPic"/>
      <hr class="my-4">
      <img src="../../assets/imgs/tDetail.png" class="detail"/>
      <p></p>

      <h1 class="display-4">examples</h1>
      <img class="t1" src="../../assets/imgs/t1.jpg"/>
      <img class="t1" src="../../assets/imgs/t2.jpg"/>
      <img class="t1" src="../../assets/imgs/t3.jpg"/>
      <img class="t1" src="../../assets/imgs/t4.jpg"/>
      <img class="t1" src="../../assets/imgs/t5.jpg"/>
      <p></p>

      <a class="btn btn-primary btn-lg" href="#" role="button" @click="next">next</a>
    </div>

  </div>
</template>

<script>
import {mapGetters} from 'vuex'

export default {
  name: 'Dashboard',
  computed: {
    ...mapGetters([
      'name'
    ])
  },
  methods:{
    next(){
      this.$router.push({name:'page4'})
    }
  },
  onload() {
  }

}
</script>

<style lang="scss" scoped>
.dashboard {
  min-height: 100vh;

  .jumbotron {
    min-height: 100vh;
    margin-bottom: 0;
    .bigPic{
      width: 40%;


    }

    img {
      margin: 60px ;
    }
  }

}
</style>
