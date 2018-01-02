<template>
    <div>
        <div class="card-container">
            <ul class="card-box">
                <li>京<i class="iconfont down-icon">&#xe660;</i></li>
                <li>Q</li>
                <li>C</li>
                <li>2</li>
                <li>L</li>
                <li>8</li>
                <li>5</li>
            </ul>
            <p class="new-car-type"><input type="checkbox"/>新能源车号码</p>
        </div>
        <ul class="card-keyboard" v-show="keyboard">
            <li>京</li>
            <li>津</li>
            <li>沪</li>
            <li>粤</li>
            <li>渝</li>
            <li>冀</li>
            <li>豫</li>
            <li>辽</li>
            <li>黑</li>
            <li>鲁</li>
            <li>湘</li>
            <li>皖</li>
            <li>苏</li>
            <li>浙</li>
            <li>鄂</li>
            <li>赣</li>
            <li>闽</li>
            <li>贵</li>
            <li>云</li>
            <li>桂</li>
            <li>晋</li>
            <li>蒙</li>
            <li>陕</li>
            <li>吉</li>
            <li>青</li>
            <li>甘</li>
            <li>藏</li>
            <li>川</li>
            <li>新</li>
            <li>宁</li>
            <li>琼</li>
            <li>港</li>
            <li>澳</li>
            <li>台</li>
            <li>军</li>
            <li class="keyboard-btn"><i class="iconfont">&#xe643;</i>切换</li>
            <li class="keyboard-btn"><i class="iconfont">&#xe61e;</i>删除</li>
        </ul>
    </div>
</template>
<script>
    export default{
        data() {
            return {
                keyboard: false//模拟键盘是否开启
            }
        }
    }
</script>
<style lang="stylus" scoped>
.card-container{
    margin: 10px 0;
    .card-box{
        display: flex;
        padding: 14px 10px;
        border: 1px solid #ccc;
        border-radius: 5px;
        li:first-child{
            border-right: 1px solid #ccc;
        }
        li{
            flex: 1;
            font-size: 14px;
            text-align: center;
            .down-icon{
                font-size: 12px;
                margin-left: 6px;
            }
        }
        li + li{
            color: #FA9D26;
            font-weight: 700;
            font-size: 16px;
        }
    }
    .new-car-type{
        margin-top: 10px;
        text-align: right;
        font-size: 14px;
        input{
            margin-right: 6px;
        }
    }
}
.card-keyboard{
    display: flex;
    width: 100%;
    justify-content: space-between;
    flex-wrap: wrap;
    background-color: #ededed;
    position: fixed;
    left: 0;
    bottom: 0;
    box-sizing: border-box;
    padding: 10px;
    li{
        width: 45px;
        height: 45px;
        line-height: 45px;
        margin-bottom: 8px;
        border: 1px solid #ccc;
        text-align: center;
        border-radius: 3px;
        font-size: 14px;
        background-color: #fff;
        i{
            color: #ccc;
            margin-right: 6px;
            font-size: 20px;
            vertical-align: middle;
        }
    }
    .keyboard-btn{
        width: 100px;
    }
}
</style>