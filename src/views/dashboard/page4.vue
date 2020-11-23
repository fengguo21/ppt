<template>
  <div class="dashboard">

    <div class="jumbotron">
      <h1 class="display-4">二维码</h1>
      <p class="lead">然而摩尔斯电码是由美国人摩尔斯在1837年被发明的，它的组成是由点dot（.）划dash（-）这两种符号所组成的。</p>

      <img src="../../assets/imgs/b1.png"/>
      <p>It uses utility classes for typography and spacing to space content out within the larger container.</p>

      <h1 class="display-4">examples</h1>
      <img src="../../assets/imgs/b1.png"/>
      <img class="t1" src="../../assets/imgs/b2.png"/>
      <p>13843076014</p>
      <p>北国风光，千里冰封，万里雪飘。望长城内外，惟余莽莽；大河上下，顿失滔滔。 山舞银蛇，原驰蜡象，欲与天公试比高。 须晴日，看红装素裹，分外妖娆。 江山如此多娇，引无数英雄竞折腰。 惜秦皇汉武，略输文采；唐宗宋祖，稍逊风骚。 一代天骄，成吉思汗，只识弯弓射大雕。 俱往矣，数风流人物，还看今朝。</p>
      <img class="t1" src="../../assets/imgs/b3.jpeg"/>
      <p>It uses utility classes for typography and spacing to space content out within the larger container.</p>
      <img class="t1" src="../../assets/imgs/b4.jpeg"/>
      <p>It uses utility classes for typography and spacing to space content out within the larger container.</p>
      <img class="t1" src="../../assets/imgs/b5.gif"/>
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
      this.$router.push({name:'page5'})
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
