<template>
    <div>
        <Panel>
            <ul :class="$style.list">
                <li :class="$style.first">
                    <router-link :to="{ name: 'home'}">
                        <img src="//img12.360buyimg.com/jrpmobile/jfs/t2842/350/3035567089/14791/5f6ff93d/577cf395N31e76288.png?width=1125&height=252">
                    </router-link>
                </li>
                <li :class="$style.end">
                    <div>
                        <img src="//img12.360buyimg.com/jrpmobile/jfs/t2971/333/1297567079/898/f2d2e00d/577dc28dNe5138337.png?width=108&height=108">
                        <p>客户端</p>
                    </div>
                    <div>
                        <img src="//img12.360buyimg.com/jrpmobile/jfs/t2971/333/1297567079/898/f2d2e00d/577dc28dNe5138337.png?width=108&height=108">
                        <p>触屏版</p>
                    </div>
                    <div>
                        <img src="//img12.360buyimg.com/jrpmobile/jfs/t2920/282/1283157010/1040/23f1430b/577cf3e5N53f740b8.png?width=108&height=108">
                        <p>电脑版</p>
                    </div>
                </li>
                <li>Copyright © 2004-2018 京东JD.com 版权所有</li>
                <li>投资有风险，购买需谨慎</li>
                <li>京东金融平台服务协议</li>
                <li>京东金融隐私政策</li>
            </ul>
        </Panel>
    </div>
</template>

<script type="text/ecmascript-6">
    import Panel from '../core/panel.vue'
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
            Panel
        }
    }
</script>

<style lang="scss" module>
    @import "../../css/element.scss";
    .list {
        @include list;
        text-align: center;
        background-color: #F5F5F5;
        li {
            font-size: 24px;
            line-height: 1.6;
            padding: 24px 32px;
            box-sizing: border-box;
            border-bottom: 1px solid #ccc;
        }
        .first {
            padding: 0;
            background-color: #fff;
            img {
                width: 100%;
            }
        }
        .end {
            @include list(row);
            padding-top: 40px;
            margin-bottom: 20px;
            justify-content: space-around;

        }
    }
</style>
