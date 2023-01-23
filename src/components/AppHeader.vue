<script>
export default {
  
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
    }
  }

  .right{
    margin-right: 30px;

    li{
      padding: 15px 25px;
    }
  } 
}

</style>