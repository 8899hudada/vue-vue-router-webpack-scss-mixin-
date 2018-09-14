<template>
    <div>
        <section :class="[panelClass,cname]">
            <h4>- {{ title }} -</h4>
            <slot></slot>
        </section>
    </div>
</template>

<script type="text/ecmascript-6">

    export default {
        props: {
            cname: {
                type: String,
                default: ''
            },
            title: {
                type: String,
                default: ''
            }
        },
        data() {
            return {
                panelClass: 'panel'
            }
        },
        computed: {},
        created() {

        },
        methods: {},
        watch: {},
        components: {}
    }
</script>

<style lang="scss">
    @import "../../css/element.scss";
    .panel {
        @include panel;
    }
</style>
