<template>
    <div :class="[btnClass,cname]">
        <slot></slot>
    </div>
</template>

<script type="text/ecmascript-6">

    export default {
        props: {
            cname: {
                type: String,
                default: ""
            }
        },
        data() {
            return {
                btnClass: 'btn'
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
    .btn {
        @include btn;
    }
</style>
