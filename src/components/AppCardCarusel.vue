<script>
export default {
    props: {
    Card: Object,
  },
  data(){
    return{
        activeImage: 0,
    }   
  },
  methods: {
        next(){
            this.activeImage++
            if(this.activeImage > this.Card.length - 1){
                this.activeImage = 0;
            }
        },
        prev(){
            this.activeImage--
            if(this.activeImage < 0){
                this.activeImage = this.Card.length - 1;
            }
        },
    }
}
</script>

<template lang="">
    <div class="thumbs">
        <div class="prev" @click="prev"></div>
        <div class="next" @click="next"></div>
    </div>
    <div v-for="(C, index) in Card" :key="index">
        <div class="cards d-flex me-3">
            <div class="content">
                <div class="d-flex aling-items-center">
                    <img :src="Card[activeImage].image" :alt="Card.title">
                </div>
                <div class="text-center">
                    <h3>{{ Card[activeImage].title }}</h3>
                    <p>{{ Card[activeImage].text }}</p>
                </div>
                <div class="d-flex justify-content-around mb-3">
                    <div class="me-2 logo-social">
                        <a href="/"><img src="/imgs/social-1.png" alt="social-1"></a>
                    </div>
                    <div class="me-2 logo-social">
                        <a href="/"><img src="/imgs/social-2.png" alt="social-2"></a>
                    </div>
                    <div class="me-2 logo-social">
                        <a href="/"><img src="/imgs/social-3.png" alt="social-3"></a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss">
    .cards{
        border: 10px solid #232a5c;
        background-image: url('/imgs/5.jpg');
        padding: 20px;

        .content{
            padding: 88px 0 40px;
        }
    }

    .thumbs{

        .prev, .next {
        width: 40px;
        height: 40px;
        margin: 10px 0;
        border-radius: 50%;
        background: #ccc;
        position: absolute;
        right: 94%;
        bottom: 50%;
        transform: translate(-50%);
        cursor: pointer;
        z-index: 999;
        }

        .next {
            bottom: 50%;
            left: 96%;
        }
    }
</style>