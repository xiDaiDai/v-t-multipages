<template>
  <div id="list">
    <div @click="showMsg">{{msg}}</div>
    <img src="../../assets/logo.png">
    <Carousel autoplay v-model="value1" loop>
      <CarouselItem>
        <div class="demo-carousel">1</div>
      </CarouselItem>
      <CarouselItem>
        <div class="demo-carousel">2</div>
      </CarouselItem>
      <CarouselItem>
        <div class="demo-carousel">3</div>
      </CarouselItem>
      <CarouselItem>
        <div class="demo-carousel">4</div>
      </CarouselItem>
    </Carousel>
    <Slider v-model="value" range></Slider>
    <a href='edit.html'>跳转edit页面</a>
  </div>
</template>

<script>
  export default {
    name: 'List',
    data(){
        return {
            msg:'hello List',
            value: [20, 50],
            value1:0
        }
    },
    methods:{
      showMsg () {
         console.log('3333')
       }
    }
  }
</script>

<style>
  #list {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }

  .demo-carousel {
    height: 200px;
    line-height: 200px;
    text-align: center;
    color: #fff;
    font-size: 20px;
    background: #506b9e;
  }
</style>
