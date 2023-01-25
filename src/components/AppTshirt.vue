<script>
export default {
    props: {
    Tshirt: Array,
  },
}
</script>

<template lang="">
    <div v-for="(item, index) in Tshirt" :key="index" class="col-xl-3 col-md-4 col-sm-6 col-12">
        <div class="product-item">
            <div class="product-inner">
                <div class="product-thumb">
                    <img :src="item.image" alt="t-shirt">
                </div>
                <div class="product-content text-center pt-3">
                    <h5 class="subtitle-white">{{ item.title }}</h5>
                    <h5 class="subtitle-white">{{ item.price }}</h5>
                    <div class="star d-flex flex-wrap justify-content-center align-items-center pb-3">
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
</template>

<style lang="scss">
    .product-inner{
        padding: 10px;
        background: #232a5c;
        transition: 0.3s all linear;

        &:hover{
            background: #ff0052;
        }

        .product-thumb{
            overflow: hidden;
            
            img{
                width: 100%;
                transition: 0.3s all linear;

                &:hover{
                    transform: scale(1.2) rotate(5deg);
                }
            }
        }
    }
</style>