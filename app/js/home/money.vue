<template>
    <div :class="$style.money">
        <Panel :title="'理财精选'">
            <div :class="$style.list">
                <div :class="$style.list_item" v-for="(item, index) in items" :key="index">
                    <h4>{{item.title}} <span>{{item.tip}}</span></h4>
                    <div>{{item.percent}}</div>
                    <p>{{item.msg}}</p>
                </div>
            </div>
        </Panel>
    </div>
</template>

<script type="text/ecmascript-6">
    import Panel from '../core/panel.vue'
    export default {
        data() {
            return {
                items:[
                    {
                        title: '定期理财',
                        tip: '90天可质押',
                        percent: '5.50%',
                        msg: '历史年化结算利率'
                    },
                    {
                        title: '年年盈',
                        tip: '理财推荐',
                        percent: '5.80%',
                        msg: '综合年化收益率'
                    },
                    {
                        title: '基智账户',
                        tip: '组合投资',
                        percent: '8%-10%',
                        msg: '止盈年化收益率'
                    },
                    {
                        title: '小白基金',
                        tip: '超短期',
                        percent: '5.00%',
                        msg: '7日年化收益率'
                    },
                ]
            }
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
    .money {
        text-align: center;
        .list {
            @include list(row);
            text-align: left;
            .list_item {
                width: 50%;
                padding-left: 32px;
                height: 218px;
                box-sizing: border-box;
                @include list;
                h4 {
                    color: #333;
                    font-weight: 700;
                    font-size: 30px;
                    display: block;
                    height: 42px;
                    line-height: 42px;
                    position: relative;
                    margin: 34px 0 16px;
                    span {
                        height: 34px;
                        line-height: 34px;
                        font-size: 22px;
                        padding: 0 8px;
                        color: #FF5155;
                        text-align: center;
                        border: 1px solid #FF5155;
                    }
                }
                div {
                    font-weight: 700;
                    font-size: 44px;
                    height: 58px;
                    line-height: 58px;
                    color: #FF5155;
                    white-space: nowrap;
                    text-overflow: ellipsis;
                    overflow: hidden;
                }
                p {
                    font-size: 24px;
                    height: 34px;
                    line-height: 34px;
                    color: #999;
                    white-space: nowrap;
                    text-overflow: ellipsis;
                    overflow: hidden;
                }
            }
        }
    }
</style>
