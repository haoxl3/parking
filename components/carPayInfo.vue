<template>
    <div class="car-pay-info-box">
        <p class="address"><i>P</i>燕东大厦停车场</p>
        <p class="park-address">车位：A区A231车位</p>
        <ul class="park-pay">
            <li>驶入：上午9：45分</li>
            <li>停留：1小时25分钟</li>
        </ul>
        <ul class="pay-btn-box clearfix">
            <li>收费：<span>20</span>元</li>
            <li><div class="pay-btn">去交费</div></li>
        </ul>
        <div class=""></div>
    </div>
</template>
<script>
export default{
    
}
</script>
<style lang="stylus" scoped>
.car-pay-info-box{
    padding: 10px 0;
}
.address{
    font-size: 16px;
    color: #FA9D26;
    margin-bottom: 10px;
    i{
        width: 26px;
        height: 26px;
        line-height: 26px;
        display: inline-block;
        border: 1px solid #ccc;
        border-radius: 50%;
        text-align: center;
        font-weight: 700;
        margin-right: 6px;
        color: #333;
    }
}
.park-address{
    font-size: 14px;
    line-height: 24px;
}
.park-pay{
    display: flex;
    padding-bottom: 10px;
    li{
        flex: 1;
        font-size: 14px;
        line-height: 24px;
    }
}
.pay-btn-box{
    border-top: 1px solid #ccc;
    border-bottom: 1px solid #ccc;
    li{
        padding: 10px 0;
        span{
            color: #FA9D26;
        }
        .pay-btn{
            border-radius: 20px;
            width: 100px;
            padding: 4px 0;
            color: #fff;
            font-size: 14px;
            text-align: center;
            background-color: #FA9D26;
        }
    }
    li:first-child{
        float: left;
        margin-top: 4px;
    }
    li:last-child{
        float: right;
    }
}
</style>