<template>
  <div class="dashboard">

    <div class="jumbotron">
      <h1 class="display-4">图灵设计的机器</h1>

      <img src="../../assets/imgs/tulingji.jpg"/>
      <p>It uses utility classes for typography and spacing to space content out within the larger container.</p>






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
