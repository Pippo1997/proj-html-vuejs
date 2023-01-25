<script>
export default {
    props: {
    Card: Array,
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
    <div v-for="(Card, index) in Card" :key="index">
        <div class="cards d-flex me-3">
            <div class="content">
                <div class="d-flex aling-items-center">
                    <img :src="Card.image" :alt="Card.title">
                </div>
                <div class="text-center">
                    <h3>{{ Card.title }}</h3>
                    <p>{{ Card.text }}</p>
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
        width: 20px;
        height: 20px;
        margin: 10px 0;
        border-radius: 50%;
        background: #ccc;
        position: absolute;
        left: 50%;
        transform: translate(-50%);
        cursor: pointer;
        z-index: 999;
    }
    }
</style>