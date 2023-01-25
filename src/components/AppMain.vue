<script>
import AppCardCarusel from './AppCardCarusel.vue'
import AppTshirt from './AppTshirt.vue';
export default {
  components: {
    AppCardCarusel,
    AppTshirt,
  },
  data() {
    return{
      Card:[
        {
          image: '/imgs/5.png',
          title: 'GAMING TEAM',
          backimg: '/imgs/5.jpg',
        },
        {
          image: '/imgs/1.png',
          title: 'DRAGON TEAM',
          backimg: '/imgs/1.jpg',
        },
        {
          image: '/imgs/5.png',
          title: 'TIGER TEAM',
          backimg: '/imgs/5.jpg',
        },
        {
          image: '/imgs/1.png',
          title: 'FROG TEAM',
          backimg: '/imgs/1.jpg',
        },
        {
          image: '/imgs/5.png',
          title: 'SHARK TEAM',
          backimg: '/imgs/5.jpg',
        },
      ],
      Tshirt:[
      {
          image: '/imgs/01 (1).jpg',
          title: 'Blue T-Shirt Here',
          price: '$380',
        },
        {
          image: '/imgs/02 (1).jpg',
          title: 'Blue T-Shirt Here',
          price: '$380',
        },
        {
          image: '/imgs/01 (1).jpg',
          title: 'Blue T-Shirt Here',
          price: '$380',
        },
        {
          image: '/imgs/02 (1).jpg',
          title: 'Blue T-Shirt Here',
          price: '$380',
        },
      ]
    }
  }
}
</script>

<template lang="">

  <!-- start section collection -->
  <section class="collection">
    <div class="container">
      <div class="top text-center">
        <p class="subtitle-rose">today's</p>
        <h2 class="subtitle-white">Our Game Collection</h2>
      </div>
      <div class="bottom">
        <div class="row g-4 justify-content-center">
          <div class="col-lg-4 col-sm-6 col-12">
            <div class="game-collection layer">
              <div class="game-collection-content d-flex align-items-center">
                <div class="vs">
                  <div class="d-flex flex-wrap justify-content-center align-items-center gap-3">
                    <div><img src="/imgs/team-1.png" alt="team-1"></div>
                    <div><img src="/imgs/vs.png" alt="vs"></div>
                    <div><img src="/imgs/team-2.png" alt="team-2"></div>
                  </div>
                </div>
                <div class="overlay">
                  <h4>Witch Sports Team</h4>
                  <div class="star d-flex flex-wrap justify-content-center align-items-center">
                  <i class="fa-solid fa-star"></i>
                  <i class="fa-solid fa-star"></i>
                  <i class="fa-solid fa-star"></i>
                  <i class="fa-solid fa-star"></i>
                  <i class="fa-solid fa-star"></i>
                </div>
                </div>
              </div>
            </div>
          </div>
          <div class="col-lg-4 col-sm-6 col-12">
            <div class="game-collection layer">
              <div class="game-collection-content d-flex align-items-center">
                <div class="vs">
                  <div class="d-flex flex-wrap justify-content-center align-items-center gap-3">
                    <div><img src="/imgs/team-1.png" alt="team-1"></div>
                    <div><img src="/imgs/vs.png" alt="vs"></div>
                    <div><img src="/imgs/team-2.png" alt="team-2"></div>
                  </div>
                </div>
                <div class="overlay">
                  <h4>Wolf Sports Team</h4>
                  <div class="star d-flex flex-wrap justify-content-center align-items-center">
                  <i class="fa-solid fa-star"></i>
                  <i class="fa-solid fa-star"></i>
                  <i class="fa-solid fa-star"></i>
                  <i class="fa-solid fa-star"></i>
                  <i class="fa-solid fa-star"></i>
                </div>
                </div>
              </div>
            </div>
          </div>
          <div class="col-lg-4 col-sm-6 col-12">
            <div class="game-collection layer">
              <div class="game-collection-content d-flex align-items-center">
                <div class="vs">
                  <div class="d-flex flex-wrap justify-content-center align-items-center gap-3">
                    <div><img src="/imgs/team-1.png" alt="team-1"></div>
                    <div><img src="/imgs/vs.png" alt="vs"></div>
                    <div><img src="/imgs/team-2.png" alt="team-2"></div>
                  </div>
                </div>
                <div class="overlay">
                  <h4>Robot Team</h4>
                  <div class="star d-flex flex-wrap justify-content-center align-items-center">
                  <i class="fa-solid fa-star"></i>
                  <i class="fa-solid fa-star"></i>
                  <i class="fa-solid fa-star"></i>
                  <i class="fa-solid fa-star"></i>
                  <i class="fa-solid fa-star"></i>
                </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="p-5 text-center">
        <button class="btn">
          <span>Browse All games </span>
          <i class="fa-solid fa-circle-play"></i>
        </button>
      </div>
    </div>
  </section>
  <!-- end section collection -->

  <!-- start about section -->
  <section class="about py-5">
    <div class="container">
      <div class="border-top">
        <div class="row">
          <div class="col-lg-6">
            <div>
              <img src="/imgs/01.png" alt="about-img" class="img-girl">
            </div>
          </div>
          <div class="col-lg-6">
            <div class="about-top">
              <p class="subtitle-rose">who we are</p>
              <h2 class="subtitle-white">we are professional team esport</h2>
            </div>
            <div class="about-bottom">
              <p>
                Distinctively provide acces mutfuncto users whereas transparent
                proceses somes ncentivize eficient functionalities rather than an
                extensible archtectur services and cross
              </p>
              <div class="about-list">
                <div class="list-item d-flex">
                  <div class="circle">
                    <img src="/imgs/icon-1.png" alt="icon-about1">
                  </div>
                  <div>
                    <h5>103K COMMUNITY EARNING</h5>
                    <p>Distinctively provide acces mutfuncto users whereas communicate leveraged services</p>
                  </div>
                </div>
              </div>
              <div class="about-list">
                <div class="list-item d-flex">
                  <div class="circle">
                    <img src="/imgs/icon-2.png" alt="icon-about2">
                  </div>
                  <div>
                    <h5>34M+ REGISTERED PLAYERS</h5>
                    <p>Distinctively provide acces mutfuncto users whereas communicate leveraged services</p>
                  </div>
                </div>
              </div>
              <div class="about-list">
                <div class="list-item d-flex">
                  <div class="circle">
                    <img src="/imgs/icon-3.png" alt="icon-about3">
                  </div>
                  <div>
                    <h5>240K STREAMS COMPLETE</h5>
                    <p>Distinctively provide acces mutfuncto users whereas communicate leveraged services</p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
  <!-- start about section -->

  <!-- start section carusel -->
  <section class="our-team">
    <div class="container-fluid">
      <div class="text-center">
        <p class="subtitle-rose">OUR TEAM PLAYERS</p>
        <h2 class="subtitle-white">MEET OUR SQUAD PLAYERS</h2>
      </div>
      <div class="carusel">
        <AppCardCarusel :Card="Card" />
      </div>
    </div>
  </section>
  <!-- end section carusel -->

  <!-- start section play -->
  <section class="play py-5">
    <div class="container">
      <div class="play-layer">
        <div class="cta d-flex">
          <div class="row align-items-center">
            <div class="col-lg-6 p-5">
              <div class="cta-content">
                <p class="subtitle-rose">Let's Play together</p>
                <h2 class="subtitle-white">JOIN <span class="color-rose">GAMER</span> ESPORTS TO BECOME
                    NEXT PRO GAMER TODAY!</h2>
                <p>
                  Distinctively provide acces mutfuncto users whereas transparent
                  proceses somes ncentivize eficient functionalities rather than an
                  extensible archtectur services and cross
                </p>
                <button class="btn">
                  <span>Join commuinity </span>
                  <i class="fa-solid fa-circle-play"></i>
                </button>
              </div>
            </div>
            <div class="col-lg-6">
              <div class="cta-thumb">
                <img src="/imgs/01 (1).png" alt="play">
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
  <!-- end section play -->

  <!-- start section our video -->
  <section class="our-video py-5">
    <div class="container">
      <div class="top text-center py-5">
        <p class="subtitle-rose">our LATEST VIDEOS</p>
        <h2 class="subtitle-white">check our live streaming</h2>
      </div>
      <div class="section-video">
        <div class="row g-4">
          <div class="col-12">
            <div class="video-top">
              <div class="row g-4 jusify-content-center">
                <div class="col-lg-6 col-12">
                  <div class="video-content">
                    <div class="video-inner">
                      <div class="video-thumb">
                        <img src="/imgs/01.jpg" alt="girl">
                        <div class="video-icon">
                          <i class="fa-solid fa-circle-play"></i>
                        </div>
                      </div>
                      <div class="video-text">
                        <div class="mb-3">
                          <a href="/" class="subtitle-white">
                            watch now 
                            <i class="fa-solid fa-circle-play"></i>
                          </a>
                        </div>
                        <h3 class="subtitle-white">2022 LVP SuperLiga Orange Summer</h3>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="col-lg-6 col-12">
                  <div class="video-content">
                    <div class="video-inner">
                      <div class="video-thumb">
                        <img src="/imgs/01.jpg" alt="girl">
                        <div class="video-icon">
                          <i class="fa-solid fa-circle-play"></i>
                        </div>
                      </div>
                      <div class="video-text">
                        <div class="mb-3">
                          <a href="/" class="subtitle-white">
                            watch now 
                            <i class="fa-solid fa-circle-play"></i>
                          </a>
                        </div>
                        <h3 class="subtitle-white">PUBG CLASSIC TOURNAMENT.</h3>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="col-12">
            <div class="video-bottom">
              <div class="row g-4 justify-content-center">
                <div class="col-xl-4 col-md-6 col-12">
                  <div class="video-content">
                    <div class="video-inner">
                      <div class="video-thumb">
                        <img src="/imgs/05.jpg" alt="girl">
                        <div class="video-icon">
                          <i class="fa-solid fa-circle-play"></i>
                        </div>
                      </div>
                      <div class="video-text">
                        <div class="mb-3">
                          <a href="/" class="subtitle-white">
                            watch now 
                            <i class="fa-solid fa-circle-play"></i>
                          </a>
                        </div>
                        <h3 class="subtitle-white">Can I add My Local Bank Account ?</h3>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="col-xl-4 col-md-6 col-12">
                  <div class="video-content">
                    <div class="video-inner">
                      <div class="video-thumb">
                        <img src="/imgs/05.jpg" alt="girl">
                        <div class="video-icon">
                          <i class="fa-solid fa-circle-play"></i>
                        </div>
                      </div>
                      <div class="video-text">
                        <div class="mb-3">
                          <a href="/" class="subtitle-white">
                            watch now 
                            <i class="fa-solid fa-circle-play"></i>
                          </a>
                        </div>
                        <h3 class="subtitle-white">LEAGUE BATTLE TOURNAMENT.</h3>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="col-xl-4 col-md-6 col-12">
                  <div class="video-content">
                    <div class="video-inner">
                      <div class="video-thumb">
                        <img src="/imgs/05.jpg" alt="girl">
                        <div class="video-icon">
                          <i class="fa-solid fa-circle-play"></i>
                        </div>
                      </div>
                      <div class="video-text">
                        <div class="mb-3">
                          <a href="/" class="subtitle-white">
                            watch now 
                            <i class="fa-solid fa-circle-play"></i>
                          </a>
                        </div>
                        <h3 class="subtitle-white">Where can I Redeem My Earnings ?</h3>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
  <!-- end section our video -->
  
  <!-- start section t-shirt -->
  <section class="t-shirt py-5">
    <div class="container">
      <div class="top text-center py-5">
        <p class="subtitle-rose">Gamer t-shirt's</p>
        <h2 class="subtitle-white">explore our products</h2>
      </div>
      <div class="bottom pb-5">
        <div class="row g-4 justify-content-center">
          <AppTshirt :Tshirt="Tshirt"/>
        </div>
      </div>
    </div>
  </section>
  <!-- end section t-shirt -->

  <!-- start sction sponsor -->
  <section class="sponsor">
    <div class="container">
      <div class="border-top">
        <div class="top text-center py-5">
          <p class="subtitle-rose">WE OUR PARTNERS</p>
          <h2 class="subtitle-white">BECOME A PARTNER of Gamer</h2>
        </div>
        <div class="bottom">
          <div class="row g-5 justify-content-center row-cols-md-5 row-cols-sm-3 row-cols-2">
            <div class="col">
              <img src="/imgs/05.png" alt="sponsor">
            </div>
            <div class="col">
              <img src="/imgs/06.png" alt="sponsor">
            </div>
            <div class="col">
              <img src="/imgs/07.png" alt="sponsor">
            </div>
            <div class="col">
              <img src="/imgs/08.png" alt="sponsor">
            </div>
            <div class="col">
              <img src="/imgs/05.png" alt="sponsor">
            </div>
            <div class="col">
              <img src="/imgs/06.png" alt="sponsor">
            </div>
            <div class="col">
              <img src="/imgs/07.png" alt="sponsor">
            </div>
            <div class="col">
              <img src="/imgs/08.png" alt="sponsor">
            </div>
          </div>
          <div class="py-5 text-center">
            <button class="btn">
              <span>Browse All games </span>
              <i class="fa-solid fa-circle-play"></i>
            </button>
          </div>
        </div>
      </div>
    </div>
  </section>
  <!-- end sction sponsor -->

  <!-- start section popular -->
  <section class="popular">
    <div class="container">
      <div class="top text-center py-5">
        <p class="subtitle-rose">OUR RECENT NEWS</p>
        <h2 class="subtitle-white">OUR MOST POPULAR BLOG POSTS</h2>
      </div>
      <div class="bottom pb-5">
        <div class="row g-4 justify-content-center row-cols-lg-2 row-cols-1">
          <div class="col">
            <div class="blog-item">
              <div class="blog-inner">
                <div class="blog-thumb pb-2">
                  <img src="/imgs/01 (3).jpg" alt="girl-popular">
                </div>
                <div class="blog-content">
                  <h3 class="subtitle-white">Distinctive redefine resource maximizing for</h3>
                  <div class="meta">

                  </div>
                  <p>
                    Uniquely conceptuaze visionary process ariwith tactical ramatica centered qualitys vectoris with outofthebox scenario is ompelling uthoritatively generate front-end niches after one
                  </p>
                  <button class="btn">
                    <span>Browse All games </span>
                    <i class="fa-solid fa-circle-play"></i>
                  </button>
                </div>
              </div>
            </div>
          </div>
          <div class="col">
            <div class="blog-item">
              <div class="blog-inner">
                <div class="blog-thumb pb-2">
                  <img src="/imgs/01 (3).jpg" alt="girl-popular">
                </div>
                <div class="blog-content">
                  <h3 class="subtitle-white">redefine resource maximizing for Distinctive</h3>
                  <div class="meta">

                  </div>
                  <p>
                    Uniquely conceptuaze visionary process ariwith tactical ramatica centered qualitys vectoris with outofthebox scenario is ompelling uthoritatively generate front-end niches after one
                  </p>
                  <button class="btn">
                    <span>Browse All games </span>
                    <i class="fa-solid fa-circle-play"></i>
                  </button>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
  <!-- start section popular -->

</template>

<style lang="scss">

////////// section collection

  .collection{
    background-color: rgba(9,14,56,255);

    .top{
      padding: 100px 0px 30px 0px;
    }
  }

  .game-collection{
    background-size: cover;
    background-position: center;
    height: 250px;
    transition: 0.3s all linear;
    position: relative;

    .overlay {
      position: absolute;
      content: "";
      visibility: hidden;
      opacity: 0;
      transition: all 0.45s cubic-bezier(0.68, -0.55, 0.27, 1.55);
      display: grid;
      place-content: center;
      left: 50%;
      top: 50%;
      transform: translate(-50%, -50%) scale(0);
      width: calc(100% - 20px);
      height: calc(100% - 20px);
      background-color: rgba(0, 0, 0, 0.8);

      h4{
        text-transform: uppercase;
        font-weight: 700;
      }

      i{
        color:  #ff0052;
      }
    }
  }

  .game-collection:hover .overlay {
    visibility: visible;
    opacity: 1;
    transform: translate(-50%, -50%) scale(1);
}

  .layer{
    margin-bottom: 30px;
    position: relative;
    z-index: 1;

    &:before{
      width: 95%;
      height: 95%;
      border: 1px solid rgba(255, 255, 255, 0.04);
      bottom: -12px;
      left: 50%;
      z-index: -1;
      transform: translateX(-50%);
      transition: 0.2s cubic-bezier(0.165, 0.84, 0.44, 1);
      border-radius: 3px;
      background-color: rgba(255, 255, 255, 0.1);
      position: absolute;
      content: ""
    }

    &:after{
      width: 90%;
      height: 90%;
      border: 1px solid rgba(255, 255, 255, 0.04);
      bottom: -22px;
      left: 50%;
      z-index: -2;
      transform: translateX(-50%);
      transition: 0.2s cubic-bezier(0.165, 0.84, 0.44, 1);
      border-radius: 3px;
      background-color: rgba(255, 255, 255, 0.1);
      position: absolute;
      content: ""
    }

    &:hover{
      transform: translateY(10px);
      box-shadow: 0 3px 20px rgb(0 0 0 / 40%);
    }
  }

  .layer:hover:after, .layer:hover:before {
    opacity: 0;
    bottom: 0;
    visibility: hidden;
}

  .game-collection-content{
      border-radius: 3px;
      background: #232a5c;
      height: 100%;
      align-items: center;
      place-content: center;
  }

////////// section about
.about{
  background-color: rgba(9,14,56,255);

  .border-top{
    padding-top: 130px;

    .img-girl{
      width: 90%;
    }
  }

  .about-list{
    margin-bottom: 25px;

    .list-item{
      gap: 20px;
    }
    
    .circle{
      width: 70px;
      height: 70px;
      display: grid;
      place-items: center;
      border-radius: 100%;
      background-color: #ff0052;
    }
  }
}

////////// section carusel

.our-team{
  background-color: rgba(9,14,56,255);
  padding: 5rem 0rem;
}

.carusel{
  padding: 1rem;
  display: flex;
  position: relative;
}

////////// section play

.play{
  background-color: rgba(9,14,56,255);
}

.cta{
  background-image: url('/imgs/bg (4).jpg');
}

.color-rose{
  color: #ff0052;
}

.play-layer{
  margin-bottom: 30px;
  transition: 0.3s all linear;
  position: relative;
  z-index: 1;

  &::before{
    width: 95%;
    height: 95%;
    border: 1px solid rgba(255, 255, 255, 0.04);
    bottom: -12px;
    left: 50%;
    z-index: -1;
    transform: translateX(-50%);
    transition: 0.2s cubic-bezier(0.165, 0.84, 0.44, 1);
    border-radius: 3px;
    background-color: rgba(255, 255, 255, 0.1);
    position: absolute;
    content: "";
  }

  &::after{
    width: 90%;
    height: 90%;
    border: 1px solid rgba(255, 255, 255, 0.04);
    bottom: -22px;
    left: 50%;
    z-index: -2;
    transform: translateX(-50%);
    transition: 0.2s cubic-bezier(0.165, 0.84, 0.44, 1);
    border-radius: 3px;
    background-color: rgba(255, 255, 255, 0.1);
    position: absolute;
    content: "";
  }

  &:hover{
      transform: translateY(10px);
      box-shadow: 0 3px 20px rgb(0 0 0 / 40%);
  }
}

.play-layer:hover:after, .play-layer:hover:before {
    opacity: 0;
    bottom: 0;
    visibility: hidden;
}

////////// section our video

.our-video{
  background-image: url('/imgs/bg (3).jpg');
}

.video-inner{
  border: 10px solid #232a5c;
  position: relative;

  img{
    width: 100%;
  }

  .video-icon{
    position: absolute;
    content: "";
    top: 45%;
    left: 45%;
    background-color: #ff0052;
    border-radius: 50%;
    width: 50px;

    i{
      font-size: 50px;
    }
  }

  .video-text{
    position: absolute;
    content: "";
    padding: 30px;
    left: 0px;
    bottom: 0px;

    a{
      padding: 8px 17px;
      margin-bottom: 10px;
      border-radius: 3px;
      background-color: #ff0052;
    }
  }
}

////////// section t-shirt

.t-shirt{
  background-color: rgba(9,14,56,255);
}

///////// section sponsor

.sponsor{
  background-color: rgba(9,14,56,255);
}

////////// section popular

.popular{
  background-image: url('/imgs/bg (2).jpg');
}

.blog-inner{
  background: rgba(35, 42, 92, 0.9);
  padding: 1rem;
}

.blog-thumb{
  overflow: hidden;

  img{
    width: 100%;
    transition: 0.3s all linear;

    &:hover{
      transform: scale(1.3);
    }
  }
}

</style>