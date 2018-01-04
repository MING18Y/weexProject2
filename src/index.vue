<template>
  <div class="wrapper" @click="update">
    <image :src="logoUrl" class="logo"></image>
    <text class="title">Hello {{target}}</text>
    <text class="desc">Now, let's use vue to build your weex app.</text>
    <button type="button" class="redirectButton" @click="redirect">Redirect</button>
  </div>
</template>

<style>
  .wrapper { align-items: center; margin-top: 120px; }
  .title { padding-top:40px; padding-bottom: 40px; font-size: 48px; }
  .logo { width: 360px; height: 156px; }
  .desc { padding-top: 20px; color:#888; font-size: 24px;}
  .redirectButton {width:300px;height:150px;font-size: 32px;text-align:center; margin:50px;}
</style>

<script>
  export default {
    data: {
      logoUrl: 'https://www.baidu.com/img/bd_logo1.png',
      target: 'World index.vue'
    },
    methods: {
      update: function (e) {
        this.target = 'Weex'
        console.log('target:', this.target)
      },
      
      redirect:function(e) {
      	window.location.href='https://www.baidu.com';
      }
      
      
    }
  }
</script>