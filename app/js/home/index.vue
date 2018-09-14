<template lang="html">
    <div>
        <Header></Header>
        <HSlider></HSlider>
        <Money></Money>
        <Product></Product>
        <Company></Company>
    </div>
</template>

<script>
    import Header from '../public/header.vue'
    import HSlider from './HSlider.vue'
    import Money from './money.vue'
    import Product from './product.vue'
    import Company from './company.vue'
    export default {
        components: {
            Header,
            HSlider,
            Money,
            Product,
            Company
        }
    }
</script>

<style lang="scss" module>
</style>
