<template>
  <div class="dashboard">

    <div class="jumbotron">
      <h1 class="display-4">小程序码</h1>
      <p class="lead">私有协议</p>

      <img src="../../assets/imgs/mini.jpg"/>

      <h1 class="display-4" style="height: 300px"></h1>
      <img class="t1" src="../../assets/imgs/mini2.jpg"/>

      <p class="lead">有36线/54线/72线   三个版本</p>

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
      this.$router.push({name:'page6'})
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
