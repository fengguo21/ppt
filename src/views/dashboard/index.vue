<template>
  <div class="dashboard">

    <div class="jumbotron">
      <h1 class="display-4">摩尔斯电码</h1>
      <p class="lead">摩尔斯电码是由美国人摩尔斯在1837年被发明的，它的组成是由点dot（.）划dash（-）这两种符号所组成的。</p>
      <hr class="my-4">
      <img src="../../assets/imgs/mose.jpeg" class="bigPic"/>
      <h1 class="display-4 exampleWrapper">example:</h1>
      <div class="example">
        <span> I am hungry</span>

        <i class="el-icon-right" style="color: green"></i>
        <span>  ..   .- --   .... ..- -. --. .-. -.--</span>

      </div>

      <a class="btn btn-primary btn-lg"  role="button" @click="next">next</a>
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
      this.$router.push({name:'page2'})
    }
  },
  onload() {
  }

}
</script>

<style lang="scss" scoped>
.dashboard {
  min-height: 100vh;
  .jumbotron{
    .bigPic{
      width: 60%;
    }

    min-height: 100vh;
    margin-bottom: 0;
    .exampleWrapper{
      margin-top: 50px;
    }
    .example{

      display: flex;
      font-size: 60px;
      align-items: center;
      span{
        margin: 80px;
      }

    }
  }

}
</style>
