<template>
  <div class="dashboard">

    <div class="jumbotron">
      <h1 class="display-4">英格玛机</h1>
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

    img {
      width: 50%;
    }
  }

}
</style>
