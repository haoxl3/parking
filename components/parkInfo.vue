<template>
    <div class="item">
        <ul class="item-top clearfix">
            <li><i class="iconfont">&#xe6ea;</i>京QC2L85</li>
            <li><i class="iconfont">&#xe64d;</i>2017年11月10日</li>
        </ul>
        <p class="address">燕东大厦停车场<i class="iconfont">&#xe602;</i></p>
        <ul class="item-info">
            <li>驶入：8点24分</li>
            <li>离开：11点49分</li>
            <li>停留：3小时25分钟</li>
        </ul>
        <ul class="money-info clearfix">
            <li>收费：17.5元</li>
            <li><span class="no-pay">去交费</span></li>
        </ul>
    </div>
</template>
<style lang="stylus" scoped>
.item{
    border-bottom: 1px solid #E8E8E8;
    padding: 20px 10px 0;
    .item-top{
        li{
            font-size: 14px;
            i{
                margin-right: 6px;
            }
        }
        li:first-child{
            float: left;
            font-size: 16px;
            color: #FA9D26;
            i{
                color: #666;
            }
        }
        li:last-child{
            float: right;
        }
    }
    .address{
        font-size: 14px;
        margin-top: 10px;
        i{
            color: #FA9D26;
        }
    }
    .item-info{
        display: flex;
        margin: 10px 0;
        li{
            flex: 1;
            color: #666;
        }
    }
    .money-info{
        padding: 10px 0;
        border-top: 1px solid #ccc;
        li:first-child{
            float: left;
        }
        li:last-child{
            float: right;
            span{
                padding: 4px 14px;
                border-radius: 20px;
                color: #fff;
            }
            .no-pay{
                background-color: #FA9D26;
            }
            .paied{
                background-color: #259B24;
            }
        }
    }
}
</style>