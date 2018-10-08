<template>
  <div id="box">
    <ul>
      <li v-for="item in imgs"><m v-bind:arr=item.im></m></li>
    </ul>
  </div>
</template>
<script>
  import m from './item'

  export default{
    components:{
      m
    },
    data:function(){
      return{
        imgs:[{im:require('../assets/img/1.jpg')},
        {im:require('../assets/img/2.jpg')},
        {im:require('../assets/img/3.jpg')},
        {im:require('../assets/img/4.jpg')},
        {im:require('../assets/img/5.jpg')},
        {im:require('../assets/img/6.jpg')},
        {im:require('../assets/img/7.png')},
        {im:require('../assets/img/8.png')}]
      }
    }
  }
</script>

<style type="text/css">
  li{
    float: left;
  }
</style>
