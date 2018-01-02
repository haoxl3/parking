<template>
    <div>
        <div class="map-container"></div>
        <div class="park-detail-box">
            <park-space-info></park-space-info>
        </div>
        <div class="app-box">
            <pay-fee></pay-fee>
            <ul class="appoint-rules">
                <li>
                    <i class="iconfont">&#xe6f0;</i>
                    预约到达时间：<span>下午2点50</span>
                </li>
                <li>
                    <i class="iconfont">&#xe60a;</i>
                    收费将以预计到达时间为起始时间，超过30分钟没有入场，则自动取消当前预约。
                </li>
                <li>
                    <input type="checkbox"/>
                    我同意《易停车用户协议》
                </li>
            </ul>
            <div class="long-btn">继续预约</div>
        </div>
    </div>
</template>
<script>
import parkSpaceInfo from '~/components/parkSpaceInfo'
import payFee from '~/components/payFee'

export default{
    components: {
        parkSpaceInfo,
        payFee
    }
}
</script>
<style lang="stylus">
.map-container{
    height: 220px;
    background-color: pink;
}
.park-detail-box{
    border-bottom: 8px solid #eee;
}
.app-box{
    padding: 10px;
    background-color: #fff;
    .appoint-rules{
        li{
            color: #666;
            margin-bottom: 6px;
            i{
                color: #666;
                margin-right: 4px;
            }
        }
        li:nth-child(2){
            color: #CBCBCB;
        }
    }
}
</style>