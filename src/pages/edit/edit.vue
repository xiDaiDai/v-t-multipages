<template>
  <div id="edit">
    <img src="../../assets/logo.png">
    <div>edit</div>
    <HelloWorld/>
  </div>
</template>

<script>
  import HelloWorld from '@/components/HelloWorld'

  export default {
    name: 'edit',
    components:{
      HelloWorld
    }
  }
</script>

<style>
  #edit {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
</style>
