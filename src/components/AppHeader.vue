<script>
import AppNavbar from './AppNavbar.vue'
export default {
  components: {
    AppNavbar,
  },
  data() {
    return{
      Menu:[
        {
          label: 'Home',
        },
        {
          label: 'Features',
        },
        {
          label: 'Achivment',
        },
        {
          label: 'Blog',
        },
        {
          label: 'Contant',
        },
      ]
    }
  }
}
</script>

<template lang="">
  <header>
    <div class="container">
      <div class="header-top">
        <div class="d-flex flex-wrap align-items-center justify-content-between">
          <ul class="left d-flex flex-wrap">
            <li>
              <i class="fa-solid fa-phone"></i>
              <span>+800-123-4567 6587</span>
            </li>
            <li>
              <i class="fa-solid fa-location-dot"></i>
              <span> Beverley, New York 224 USA</span>
            </li>
          </ul>
          <ul class="right d-flex flex-wrap">
            <li>
              <a href="/"><i class="fa-brands fa-facebook-messenger"></i></a> 
            </li>
            <li>
              <a href="/"><i class="fa-brands fa-twitter"></i></a> 
            </li>
            <li>
              <a href="/"><i class="fa-brands fa-vimeo-v"></i></a> 
            </li>
            <li>
              <a href="/"><i class="fa-brands fa-skype"></i></a> 
            </li>
            <li>
              <a href="/"><i class="fa-solid fa-rss"></i></a> 
            </li>
          </ul>
        </div>
      </div>
      <div class="header-bottom">
        <div class="d-flex flex-wrap align-items-center justify-content-between">
          <div class="logo">
            <img src="/imgs/logo.png" alt="logo">
          </div>
          <div class="menu d-flex">
            <AppNavbar :Menu="Menu"/>
            <a href="/" class="login">
              <i class="fa-solid fa-user"></i>
              <span>LOG IN</span>
            </a>
            <a href="/" class="sing-up">
              <i class="fa-solid fa-users"></i>
              <span>SING IN</span>
            </a>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<style lang="scss">
@use '../styles/partials/variable' as *;

.header-top{
  border-bottom: 1px solid rgba(255, 255, 255, 0.1);

  .left{
    margin-left: 30px;

    li{
      padding: 15px 25px;

      &::after{
        content: "";
        height: 120%;
        width: 1px;
        background-color: rgba(255, 255, 255, 0.1);
        left: -20px;
        top: -7px;
        transform: rotate(-25deg);
      }
    }
  }

  .right{
    margin-right: 30px;

    li{
      padding: 15px 25px;

      &::after{
        content: "";
        height: 120%;
        width: 1px;
        background-color: rgba(255, 255, 255, 0.1);
        right: 0;
        top: -5px;
        transform: rotate(25deg);
      }
    }
  } 
}

.header-bottom{

  .menu{
    margin-right: 30px;

    .login{
      padding: 15px;
      color: #ff0052;
      border-radius: 2px 0 0 2px;

      &::before{
        content: "";
        bottom: 0;
        left: 1px;
        height: 2px;
        width: 100%;
        background: #ff0052;
      }
    }

    .sing-up{
      padding: 15px;
      color: white;
      border-radius: 0 2px 2px 0;
      background: #ff0052;

      &::before{
        content: "";
        bottom: 0;
        left: 1px;
        height: 2px;
        width: 100%;
        background:white;
        border-radius: 2px;
      }

      &::after{
        content: "";
        bottom: 0;
        right: -1px;
        width: 2px;
        height: calc(100% - 2px);
        background:white;
      }
    }
  }
}

</style>