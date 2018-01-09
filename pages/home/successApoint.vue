<template>
    <div class="app-success-container">
        <m-header><span>预约车位</span></m-header>
        <section class="appoint-info">恭喜您！您已成功为您预约车位！</section>
        <park-info></park-info>
        <ul class="success-operate">
            <li>
                <div class="btn cancel"><i class="iconfont">&#xe6c4;</i>取消预约</div>
            </li> 
            <li>
                <div class="btn navigate"><i class="iconfont">&#xe66d;</i>开始导航</div>
            </li> 
        </ul>
        <div class="qrcode-container">
            <div class="qrcode-box"></div>
            <p>进入停车场时出示此二维码，您将享受快速通行服务。感谢您使用易停车服务！</p>
            <h4>服务电话：<span>400-000-000</span></h4>
        </div>
    </div>
</template>
<script>
import mHeader from '~/components/mHeader'
import parkInfo from '~/components/parkInfo' 
export default{
    components: {
        mHeader,
        parkInfo
    }
}
</script>
<style lang="stylus">
.app-success-container{
    background-color: #fff;
    border-bottom: 1px solid #ccc;
    .appoint-info{
        text-align: center;
        font-size: 16px;
        padding: 20px 0;
        border-bottom: 1px solid #ccc;
    }
    .success-operate{
        display: flex;
        padding: 10px 0;
        li{
            flex: 1;
            padding: 6px 20px;
            .btn{
                width: 100%;
                height: 30px;
                line-height: 30px;
                border-radius: 20px;
                text-align: center;
                font-size: 14px;
                i{
                    margin-right: 4px;
                    vertical-align: middle;
                }
            }
            .cancel{
                background-color: #ccc;
            }
            .navigate{
                background-color: #FF9D00;
            }
        }
        li + li{
            border-left: 1px solid #eee;
        }
    }
    .qrcode-container{
        background-color: #fff;
        border-top: 8px solid #eee;
        padding: 10px 0;
        text-align: center;
        .qrcode-box{
            width: 160px;
            height: 160px;
            background-color: pink;
            margin: 0 auto 10px;
        }
        p{
            line-height: 20px;
            color: #444;
            padding: 0 14%;
            font-size: 14px;
        }
        h4{
            color: #666;
            margin-top: 6px;
            span{
                color: #FA9D26;
            }
        }
    }
}
</style>