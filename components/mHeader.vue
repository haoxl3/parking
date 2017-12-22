<template>
    <header>
        <i class="iconfont return" v-show="isReturn" @click="goBack">&#xe619;</i>
        <slot>易停车</slot>
    </header>            
</template>
<script>
export default {
    props: {
        isReturn: {
            type: Boolean,
            default: true
        }
    },
    methods: {
        goBack() {
            this.$router.go(-1)
        }
    }
}
</script>
<style lang="stylus">
    $height = 3rem;
    header{
        height: $height;
        line-height: $height;
        background-color: #555555;
        color: #fff;
        position: relative;
        text-align: center;
        font-size: 1.2rem;
        .return{
            position: absolute;
            top: 0;
            bottom: 0;
            left: 10px;
            cursor: pointer;
        }
    }
</style>