<template>
    <div>
        <m-header><span>预约车位</span></m-header>
        <park-space-info></park-space-info>
        <div class="parking-detail-box">
            <div class="parking-title">
                <p><i class="iconfont">&#xe662;</i>北京龙越物业管理公司</p>
                <p><i class="iconfont">&#xe602;</i>北京市朝阳区望京万红西街2号</p>
            </div>
            <ul class="info-grid">
                <li>
                    <p>地面车位</p>
                    <p>78</p>
                </li>
                <li>
                    <p>地下车位</p>
                    <p>0</p>
                </li>
                <li>
                    <p>营业时间</p>
                    <p>全天</p>
                </li>
                <li>
                    <p>优惠政策</p>
                    <p>免16分钟</p>
                </li>
            </ul>
            <ul class="charge-grid">
                <li>
                    <h3>白天<span>(早7点至晚9点)</span></h3>
                    <p>
                        <span>小型车</span>
                        <span>1.25元/15分钟</span>
                    </p>
                    <p>
                        <span>大型车</span>
                        <span>2.5元/15分钟</span>
                    </p>
                </li>
                <li>
                    <h3>夜间<span>(晚9点至早7点)</span></h3>
                    <p>
                        <span>小型车</span>
                        <span>1.25元/15分钟</span>
                    </p>
                    <p>
                        <span>大型车</span>
                        <span>2.5元/15分钟</span>
                    </p>
                </li>
            </ul>
        </div>
        <div class="lot-img">停车场平面图</div>
    </div>
</template>
<script>
import parkSpaceInfo from '~/components/parkSpaceInfo'
import mHeader from '~/components/mHeader'
export default{
    components: {
        parkSpaceInfo,
        mHeader
    }
}
</script>
<style lang="stylus">
.parking-detail-box{
    padding: 0 10px;
    background-color: #fff;
    margin: 8px 0;
    .parking-title{
        padding: 10px 0;
        p{
            line-height: 20px;
            font-size: 14px;
            i{
                color: #FA9D26;
                margin-right: 6px;
            }
        }
    }
    .info-grid{
        display: flex;
        padding: 10px 0;
        border-top: 1px solid #ccc;
        border-bottom: 1px solid #ccc;
        li{
            flex: 1;
            text-align: center;
            p{
                line-height: 30px;
                font-size: 14px;
            }
            p:first-child{
                color: #ccc;
            }
        }
        li+li{
            border-left: 1px solid #ccc;
        }
    }
    .charge-grid{
        display: flex;
        padding: 10px 0;
        li{
            flex: 1;
            padding: 0 4px;
            h3{
                text-align: center;
                margin-bottom: 10px;
                span{
                    color: #ccc;
                }
            }
            p{
                display: flex;
                line-height: 26px;
                justify-content: space-between;
                span{
                    flex: 1;
                }
            }
        }
        li:first-child{
            border-right: 1px solid #ccc;
        }
    }
}
.lot-img{
    height: 200px;
    margin-top: 8px;
    background-color: #fff;
}
</style>