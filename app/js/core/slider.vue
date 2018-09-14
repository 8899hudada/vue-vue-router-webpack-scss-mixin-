<template>
    <div>
        <section :class="cname">
            <swiper :options="options" :not-next-tick="options.notNextTick">
                <swiperSlide v-for="(item, index) in items" :key="index">
                    <router-link :to="{ name: item.href}">
                        <img :src="item.src">
                    </router-link>
                </swiperSlide>
                <div class="swiper-pagination"  slot="pagination" v-if="options.pagination"></div>
            </swiper>
        </section>
    </div>
</template>

<script type="text/ecmascript-6">
    import { swiper, swiperSlide } from 'vue-awesome-swiper'
    export default {
        props: {
            cname: {
                type: String,
                default: ''
            },
            options: {
                type: Object,
                default() {
                    return {
                        autoplay: true,
                        loop: true,
                        pagination: {
                            el: '.swiper-pagination'
                        },
                        notNextTick: false
                    }
                }
            },
            items: {
                type: Array,
                default() {
                    return ['','']
                }
            }
        },
        data() {
            return {}
        },
        computed: {},
        created() {

        },
        methods: {},
        watch: {},
        components: {
            swiper,
            swiperSlide
        }
    }
</script>

<style lang="css">
    @import "~swiper/dist/css/swiper.css";

</style>
