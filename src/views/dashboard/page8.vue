<template>
  <div class="dashboard">

    <div class="jumbotron">
      <h1 class="display-4">图灵设计的机器</h1>
<<<<<<< HEAD
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
=======
      <p class="lead">艾伦·麦席森·图灵（英语：Alan Mathison Turing，1912年6月23日—1954年6月7日），英国数学家、逻辑学家，被称为计算机科学之父，人工智能之父。</p>

      <img src="../../assets/imgs/tulingji.jpg"/>
      <h1 class="display-4"></h1>
      <div style="font-size: 40px">
        <p>明文 W  E  T  T  E  R<p/>
        <p>密文 E R K M G W</p>
      </div>

      <p></p>


      <a class="btn btn-primary btn-lg" href="#" role="button" @click="next">next</a>
    </div>
>>>>>>> 90e615328b44e6a776db2115fe27a3067a9e87ef

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
<<<<<<< HEAD
      width: 50%;
=======
      width: 30%;
>>>>>>> 90e615328b44e6a776db2115fe27a3067a9e87ef
    }
  }

}
</style>
