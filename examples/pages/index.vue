<template>
  <div class="m-index">
    <div class="m-ban">
      <img src="../assets/img/logo.png">
      <p class="mt40">Xue-UI</p>
      <p class="mt10">一款自己用的前端 UI 组件库</p>
      <div class="df s-jcc mt30">
        <router-link :to="{name: 'giud'}">
          <xu-button class="mr20">开始使用</xu-button>
        </router-link>
        <a target="_blank" class="btn-github" href="https://github.com/linwens/xueui-demo">
          <xu-button>GitHub</xu-button>
        </a>
      </div>
    </div>
    <div class="m-intro">
      <div class="df">
        <xu-icon class="xu-icon-taobao fs-24"></xu-icon>
        <div>
          <h2>公司内部系统</h2>
          <p>可以作为其他UI库组件的补充</p>
        </div>
      </div>
      <div class="df">
        <xu-icon class="xu-icon-taobao fs-24"></xu-icon>
        <div>
          <h2>个人维护</h2>
          <p></p>
        </div>
      </div>
      <div class="df">
        <xu-icon class="xu-icon-taobao fs-24"></xu-icon>
        <div>
          <h2>使用需谨慎</h2>
          <p></p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default{
    data () {
      return {
        height: document.documentElement.clientHeight
      }
    }
  }
</script>
<style type="text/scss" lang="scss">
  .m-index {
    .m-ban {
      width: 960px;
      margin: 0 auto;
      text-align: center;
      padding: 100px 0;
      p{
        color: #6a8bad;
        &:nth-child(2) {
          font-size: 40px;
        }
        &:nth-child(3) {
          font-size: 26px;
        }
      }
    }
    .separate-panel{
      position: relative;
      .about{
        position: absolute;
        width: 100%;
        height: 200px;
        top: 20px;
        z-index: 9;
        background: #fff;
        text-align: center;
        a {
          color: #fff;
          background-image: linear-gradient(90deg, #00AEFF 0%, #3369E7 100%);
          box-shadow: 0 2px 6px 0 rgba(51,105,231,0.4);
          display: inline-block;
          width: 190px;
          height: 56px;
          margin: 0 35px;
          font-size: 18px;
          line-height: 56px;
          border-radius: 28px;
          transition: all .3s;
          cursor: pointer;
        }
        .btn-github{
          color: #316DE9;
          border: 1px solid #2F6EE9;
          background: #fff;
          box-shadow: none;
        }
      }
    }
    .separate-panel:after{
      content: '';
      display: block;
      position: absolute;
      top: -80px;
      width: 100%;
      height: 250px;
      background: #fff;
      box-shadow: 0 -4px 30px 0 #DFE1E6;
      transform: skewY(-4deg);
    }
  }
</style>
