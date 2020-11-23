<template>
  <div class="dashboard">

    <div class="jumbotron">
      <h1 class="display-4">图灵设计的机器</h1>
      <p class="lead">然而摩尔斯电码是由美国人摩尔斯在1837年被发明的，它的组成是由点dot（.）划dash（-）这两种符号所组成的。</p>

      <img src="../../assets/imgs/tulingji.jpg"/>
      <p>It uses utility classes for typography and spacing to space content out within the larger container.</p>


      <a class="btn btn-primary btn-lg" href="#" role="button" @click="next">Learn more</a>
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
  methods:{
    next(){
      this.$router.push({name:'pageFive'})
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
      width: 50%;
    }
  }

}
</style>
