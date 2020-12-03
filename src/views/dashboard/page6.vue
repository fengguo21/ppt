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
<<<<<<< HEAD
        <h1 class="display-4" style="margin: 540px"></h1>
        <img src="../../assets/imgs/mimabiao3.jpg"/>
=======

        <h1 class="display-4" style="margin: 540px"></h1>
        <img src="../../assets/imgs/mimabiao3.jpg"/>
        <h1 class="display-4" style="margin: 540px"></h1>
        <div class="example" >
          <span>This is Hong Tao’s latest movies. I like Hong Tao. He’s made some great movies over the years. Unfortunately, this is his worst movie. If you’re looking for entertainment, stay at home and watch TV. Yellow River Fisherman is too long, and it’s really boring. It does have a few good features, though.I thought the fisherman’s wife was really funny. Amy Kate Photography Be sure to see this exhibition at the Lido Gallery. Amy Kim is one of the best-known Chinese photographers in the world today, and some of her most famous photos are on display in this exhibition. She really has something for everyone. There are many great photos of people and of the countryside, The few city photographs are less successful. I see the same things every day and they don’t interest me as much. But this is a great show from a world-class photographer. Whatever you do, don’t miss this exhibition. Wild and Windy Over the years, we’re seen musical groups with pretty strange names come and go. Few have stranger names than this band. As the name suggests, the band has lots of energy. And they play the kind of music that I love to hear. Every song is really loud and you often can’t understand the words, but this is okay because the lyrics aren’t very good. However, these are musicians who make us happy—even on a Monday morning!</span>

          <!--          <i class="el-icon-right" style="color: green"></i>-->
          <!--          <span> S CY RIZEFN</span>-->
        </div>
>>>>>>> 90e615328b44e6a776db2115fe27a3067a9e87ef
      </div>





<<<<<<< HEAD
      <a class="btn btn-primary btn-lg" href="#" role="button" @click="next">Learn more</a>
=======
      <a class="btn btn-primary btn-lg" href="#" role="button" @click="next">next</a>
>>>>>>> 90e615328b44e6a776db2115fe27a3067a9e87ef
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
<<<<<<< HEAD
=======
      margin: 30px 100px;
>>>>>>> 90e615328b44e6a776db2115fe27a3067a9e87ef
      width: 50%;
    }
  }

}
</style>
