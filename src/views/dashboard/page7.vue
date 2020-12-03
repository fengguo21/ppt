<template>
  <div class="dashboard">

    <div class="jumbotron">
      <h1 class="display-4">英格玛机</h1>
<<<<<<< HEAD
      <p class="lead">然而摩尔斯电码是由美国人摩尔斯在1837年被发明的，它的组成是由点dot（.）划dash（-）这两种符号所组成的。</p>

      <img src="../../assets/imgs/yinggemaji.jpg"/>
      <img src="../../assets/imgs/zhuanzi.jpg"/>
      <img src="../../assets/imgs/zhuanzi2.jpg"/>
      <img src="../../assets/imgs/fanshe.jpg"/>
      <img src="../../assets/imgs/xianban.jpg"/>
      <p>It uses utility classes for typography and spacing to space content out within the larger container.</p>

      <h1 class="display-4">examples</h1>
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
      <p class="lead">一种用于加密与解密文件的密码机。是对二战时期纳粹德国使用的转子机械加解密机器</p>

      <img class="bigPic" src="../../assets/imgs/yinggemaji.jpg"/>
      <h1 class="display-4" style="margin: 300px;"></h1>

      <img src="../../assets/imgs/zhuanzi.jpg"/>
      <p style="font-size: 50px;margin-left: 300px">组合数：26*26*26</p>
      <h1 class="display-4" style="margin: 300px;"></h1>
      <img class="explain" src="../../assets/imgs/explain.png"/>
      <img src="../../assets/imgs/fanshe.jpg"/>
      <h1 class="display-4" style="margin: 300px;"></h1>
      <img src="../../assets/imgs/xianban.jpg"/>
      <p style="font-size: 50px;margin-left: 300px">组合数：26*25*24*23*22*21*20*19*18  </p>
      <p></p>

      <h1 class="display-4"></h1>
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
      this.$router.push({name:'page8'})
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
<<<<<<< HEAD
    min-height: 100vh;
    margin-bottom: 0;
=======
    img{
      margin: 30px 100px;
    }
    .explain{
      width: 50px;
    }

    min-height: 100vh;
    margin-bottom: 0;
    .bigPic{
      width: 30%;
    }
>>>>>>> 90e615328b44e6a776db2115fe27a3067a9e87ef

    img {
      width: 50%;
    }
  }

}
</style>
