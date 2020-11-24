<template>
  <div class="dashboard">

    <div class="jumbotron">
      <h1 class="display-4" style="margin-bottom: 40px">加密</h1>

      <img src="../../assets/imgs/mimabiao.jpg"/>
      <h1 class="display-4" style="margin: 40px 0">example</h1>
      <div class="example" >
        <span> I am hungry</span>

        <i class="el-icon-right" style="color: green"></i>
        <span> S CY RIZEFN</span>
      </div>
      <h2 class="display-4" style="margin-bottom: 40px;margin-top: 300px">字母频率表</h2>
      <img src="../../assets/imgs/tongji.png"/>
      <h1 class="display-4" style="margin-bottom: 40px;margin-top: 300px"></h1>
      <div>
        <img src="../../assets/imgs/mimabiao2.jpg"/>
        <h1 class="display-4" style="margin: 540px"></h1>
        <img src="../../assets/imgs/mimabiao3.jpg"/>
      </div>





      <a class="btn btn-primary btn-lg" href="#" role="button" @click="next">Learn more</a>
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
      this.$router.push({name:'page7'})
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
    .example{
      display: flex;
      font-size: 60px;
      align-items: center;
      span{
        margin: 80px;
      }
    }

    img {
      width: 50%;
    }
  }

}
</style>
