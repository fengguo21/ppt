<template>
  <div class="dashboard">

    <div class="jumbotron">
      <h1 class="display-4">二维码</h1>
      <p class="lead">二维码又称二维条码，常见的二维码为QR Code，QR全称Quick Response，是一个近几年来移动设备上超流行的一种编码方式，它比传统的Bar Code条形码能存更多的信息</p>

      <p></p>

      <!--      <h1 class="display-4">examples</h1>-->
      <div class="examples" style="margin-top: 200px;margin-bottom: 100px">
        <div class="item">
          <img src="../../assets/imgs/b1.png"/>
          <p>13843076014</p>
        </div>
        <div class="item">
          <img  src="../../assets/imgs/b2.png"/>
          <p>北国风光，千里冰封，万里雪飘。望长城内外，惟余莽莽；大河上下，顿失滔滔。 山舞银蛇，原驰蜡象，欲与天公试比高。 须晴日，看红装素裹，分外妖娆。 江山如此多娇，引无数英雄竞折腰。 惜秦皇汉武，略输文采；唐宗宋祖，稍逊风骚。
            一代天骄，成吉思汗，只识弯弓射大雕。 俱往矣，数风流人物，还看今朝。</p>
        </div>


      </div>

      <h1 class="display-4">examples</h1>
      <div class="decorations">
        <img class="t1" src="../../assets/imgs/b3.jpeg"/>
        <img class="t1" src="../../assets/imgs/b4.jpeg"/>
        <img class="t1" src="../../assets/imgs/b6.jpg"/>
        <img class="t1" src="../../assets/imgs/b7.png"/>
      </div>



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
      this.$router.push({name: 'page5'})
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
    .decorations{
      display: flex;
      img{
        width: 300px;
        height: 250px;
        margin-right: 100px;
      }
    }
    .examples{
      display: flex;
      justify-content: space-between;
      margin: 100px;
      .item{
        margin-right: 300px;
        //flex: 1;

        img{
          width: 300px;
          margin-bottom: 60px;
        }
      }
      img{
        width: 50%;
      }
    }

    //.bigPic {
    //  width: 40%;
    //  margin: 60px;
    //}

    //img {
    //  width: 50%;
    //}
  }

}
</style>
