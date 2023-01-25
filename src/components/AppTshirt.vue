<script>
export default {
    props: {
    Tshirt: Array,
  },
}
</script>

<template lang="">
    <div v-for="(item, index) in Tshirt" :key="index">
        <div class="product-item">
            <div class="product-inner">
                <div class="product-thumb">
                    <img :src="item.image" alt="t-shirt">
                </div>
                <div class="product-content">
                    <h5>{{ item.title }}</h5>
                    <h5>{{ item.price }}</h5>
                    <div>

                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss">
    
</style>