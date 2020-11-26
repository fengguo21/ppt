<template>
  <div class="dashboard">

    <div class="jumbotron">
      <h1 class="display-4">图灵设计的机器</h1>
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
      width: 30%;
    }
  }

}
</style>
