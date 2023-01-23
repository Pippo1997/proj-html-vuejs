<script>
export default {
  props: {
    Menu: Array
  }
}
</script>

<template lang="">
  <nav class="d-flex flex-wrap align-items-center justify-content-between">
    <ul class="d-flex">
        <li v-for="(item, index) in Menu" :key="index">
            <a href="/">{{ item.label }}</a>
        </li>
    </ul>
  </nav>
</template>

<style lang="scss">

    nav{
        margin-right: 30px;

        li{
            color: #fff;
            font-size: 1rem;
            font-weight: 700;
            padding: 15px 22px;
            text-transform: uppercase;
        }
    }
</style>