<script>
export default {
    props: {
    Card: Array,
  },
}
</script>

<template lang="">
    <div v-for="(Card, index) in Card" :key="index">
        <div class="cards d-flex me-3">
            <!-- <div class="background">
                <img :src="Card.backimg" alt="background">
            </div> -->
            <div class="content">
                <div class="d-flex aling-items-center">
                    <img :src="Card.image" alt="card">
                </div>
                <div class="text-center">
                    <h3>{{Card.title}}</h3>
                    <p>{{Card.text}}</p>
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
        padding: 30px;

        .content{
            padding: 88px 0 40px;
        }
    }
</style>