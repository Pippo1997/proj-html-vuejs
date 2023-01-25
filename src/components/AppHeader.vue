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

  <!-- start scroll -->
  <a href="scroll" class="scroll-top">
    <i class="fa-solid fa-arrow-up"></i>
  </a>
  <!-- end scroll -->

  <!-- start header -->
  <header id="scroll">
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
  <!-- end header -->

  <!-- start jumbotron -->
  <div class="jumbo">
    <div class="banner">
      <div class="container">
        <div class="row">
          <div class="col-lg-6 col-md-12"> 
            <h1>Online Game</h1>
            <h2 class="subtitle-white">Genuine Money Transaction</h2>
            <p>Assertively communicate an expanded array of mindshare rather than diverse technologies for magnetic applications eamlessly virtual then Conveniently monetize synergistic human capital</p>
            <button class="btn">
              <span>join us today</span> 
              <i class="fa-solid fa-circle-play"></i>
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
  <!-- end jumbotron -->

</template>

<style lang="scss">
@use '../styles/partials/variable' as *;

///////// scroll

.scroll-top{
  bottom: 5%;
  opacity: 1;
  position: fixed;
  right: 5%;
  z-index: 99;
  transition: all 0.5s ease 0s;

  i{
    width: 40px;
    height: 40px;
    line-height: 40px;
    border-radius: 50%;
    color: #fff;
    background: #ff0052;
    font-size: 1.25rem;
    transition: 0.3s all linear;
    text-align: center;

    &:hover{
      transform: translateY(-10px);
      box-shadow: 0px 5px 20px 0px rgb(255 0 82 / 50%);
    }
  }
}

////////// header

header{
  position: absolute;
  z-index: 999;
  width: 100%;
  content: "";
  background: rgba(35, 42, 92, 0.3);
  backdrop-filter: blur(20px);
}

.header-top{
  border-bottom: 1px solid rgba(255, 255, 255, 0.1);

  .left{
    margin: 0 -55px;

    li{
      padding: 15px 25px;
      margin-left: 30px;
      position: relative;

      &:after{
        content: "";
        height: 120%;
        width: 1px;
        background-color: rgba(255, 255, 255, 0.1);
        left: -20px;
        top: -7px;
        transform: rotate(-25deg);
        position: absolute;
      }
    }
  }

  .right{
    margin: 0px -14px;

    li{
      padding: 15px 25px;
      position: relative;

      &:after{
        content: "";
        height: 115%;
        width: 1px;
        background-color: rgba(255, 255, 255, 0.1);
        right: 0;
        top: -5px;
        transform: rotate(25deg);
        position: absolute;
      }
    }
  } 
}

.header-bottom{

  .menu{

    .login{
      padding: 15px;
      background-color: white;
      color: #ff0052;
      border-radius: 2px 0 0 2px;
      position: relative;

      &:before{
        content: "";
        bottom: 0;
        left: 1px;
        height: 2px;
        width: 100%;
        background: #ff0052;
        position: absolute;
      }
    }

    .sing-up{
      padding: 15px;
      color: white;
      border-radius: 0 2px 2px 0;
      background: #ff0052;
      position: relative;

      &:before{
        content: "";
        bottom: 0;
        left: 1px;
        height: 2px;
        width: 100%;
        background:white;
        border-radius: 2px;
        position: absolute;
      }

      &:after{
        content: "";
        bottom: 0;
        right: -1px;
        width: 2px;
        height: calc(100% - 2px);
        background:white;
        position: absolute;
      }
    }
  }
}

////////// jumbotron

.jumbo{
  position: relative;
  width: 100%;
  height: 100%;
  z-index: 1;
  background-image: url('/imgs/bg.jpg');
  background-size: cover;

  .banner{
    padding: 350px 0 240px;

    h1{
      text-transform: uppercase;
      font-weight: 700;
      font-size: 5rem;
      text-shadow: 2px 2px 2px rgb(255 0 82 / 90%);
    }
  }
}

</style>