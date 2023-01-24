<script>
export default {
  
}
</script>

<template lang="">

  <!-- start section colllection -->
  <section class="collection">
    <div class="container">
      <div class="top">
        <p>today's</p>
        <h2>Our Game Collection</h2>
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
          <div class="col-lg-4 col-sm-6 col-12"></div>
          <div class="col-lg-4 col-sm-6 col-12"></div>
        </div>
      </div>
      <div class="mt-5 text-center">
        <button class="btn">
          <span>Browse All games </span>
          <i class="fa-solid fa-circle-play"></i>
        </button>
      </div>
    </div>
  </section>
  <!-- end section colllection -->

</template>

<style lang="scss">

  .collection{
    background-color: rgba(9,14,56,255);
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

</style>