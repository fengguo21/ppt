<template>
  <div class="dashboard">

    <div class="jumbotron">
      <h1 class="display-4">布莱叶盲文</h1>
      <p class="lead">由法国盲人路易·布莱尔于1824年创造的，故国际上通称为“布莱尔（Braille）”。</p>
      <hr class="my-4">
      <img src="../../assets/imgs/bra.png"/>
      <h1 class="display-4" style="margin-top: 200px">书籍</h1>
      <img src="../../assets/imgs/bra2.jpeg"/>
      <p></p>
      <a class="btn btn-primary btn-lg" href="#" role="button" @click="next">next</a>
    </div>
    <!--    <el-carousel :interval="4000" height="800px" >-->
    <!--      <el-carousel-item>-->
    <!--        <img src="../../assets/imgs/mos.jpeg"/>-->
    <!--        <h3 class="medium">1</h3>-->
    <!--      </el-carousel-item>-->
    <!--      <el-carousel-item >-->
    <!--        <img src="../../assets/imgs/bra.jpg"/>-->
    <!--        <h3 class="medium">2</h3>-->
    <!--      </el-carousel-item>-->
    <!--      <el-carousel-item >-->
    <!--        <img src="../../assets/imgs/mos.jpeg"/>-->
    <!--        <h3 class="medium">3</h3>-->
    <!--      </el-carousel-item>-->
    <!--      <el-carousel-item >-->
    <!--        <img src="../../assets/imgs/mos.jpeg"/>-->
    <!--        <h3 class="medium">4</h3>-->
    <!--      </el-carousel-item>-->
    <!--    </el-carousel>-->

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
  methods: {
    next() {
      this.$router.push({name: 'page3'})
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

    img {
      width: 60%;
      margin: 60px ;
    }
  }

}
</style>
