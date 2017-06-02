<template>
<div>
  <div class="main-body"></div>
  <div class="wrapper">
        <div class="container">
            <image class="top-line" src=""></image>
            <image class="tab-icon" src="../images/home.png"></image>
            <text class="tab-text">首页</text>
        </div>
        <div class="container">
            <image class="top-line" src=""></image>
            <image class="tab-icon" src="../images/internet_news.png"></image>
            <text class="tab-text">动态</text>
        </div>
        <div class="container">
            <image class="top-line" src=""></image>
            <image class="tab-icon" src="../images/my_info.png"></image>
            <text class="tab-text">我的</text>
        </div>
    </div>
</div>
    
</template>

<style>
.main-body{
  bottom: 0;
  left: 0;
  right: 0;
  width: 100%;
  height: 0.6rem;
}
.wrapper{
    display: flex;
    flex-direction: row;
    position: fixed;
    bottom: 0;
    left: 0;
    right: 0;
    width: 100%;
    overflow: hidden;
    height: 0.6rem;
    background: #ffffff;
    border-top: 0.01rem solid #e4e4e4;
}
.container{
    display: flex;
    flex: 1;
    text-align: center;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 100%;
}
.top-line {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 0.02rem;
  }

  .tab-icon {
    margin-top: 0.05rem;
    width: 0.30rem;
    height: 0.28rem;
  }

  .tab-text {
    margin-top: 0.02rem;
    text-align: center;
    font-size: 0.14rem;
  }
</style>

<script>
  export default {
    data: {
      logoUrl: '../assets/weex_logo_blue@3x.png',
      target: 'World'
    },
    methods: {
      update: function (e) {
        this.target = 'Weex'
        console.log('target:', this.target)
      }
    }
  }
</script>
