<template>
    <div :class="$style.header">
        <span :class="$style.left">
            <em>注册</em> &nbsp; | &nbsp; <em>注册</em>
        </span>
        <Btn :class="$style.btnDownload">APP下载</Btn>
    </div>
</template>

<script type="text/ecmascript-6">
    import Btn from '../core/btn.vue'
    export default {
        data() {
            return {}
        },
        computed: {},
        created() {

        },
        methods: {},
        watch: {},
        components: {
            Btn
        }
    }
</script>

<style lang="scss" module>
    .header {
        color: #666;
        height: 100px;
        line-height: 100px;
        position: fixed;
        top: 0;
        left: 0;
        right: 0;
        font-size: 32px;
        background: #fff url(//m.jr.jd.com/spe/qyy/main/images/jr-logo.png) center center no-repeat;
        -webkit-background-size: auto 50%;
        background-size: auto 50%;
        z-index: 100;
        .left {
            font-size: 28px;
            height: 30px;
            line-height: 30px;
            margin: 17px 0 0 18px;
        }
        .btnDownload {
            float: right;
            font-size: 24px;
            min-width: 120px;
            height: 56px;
            line-height: 56px;
            border-radius: 4px;
            border-width: 0;
            padding: 0;
            margin: 28px 24px 0 0;
        }
    }
</style>
