<template>
    <div class="footer-container">
        <ul class="clearfix">
            <li class="car-position">
                <i class="iconfont">&#xe642;</i>
                <span>你的爱车停放在燕东大厦科技园2号楼3号停车场</span>
            </li>
            <li>
                <i class="iconfont icon-weather">&#xe767;</i>
                <span>21度</span>
            </li>
            <li>今日不限行</li>
        </ul>
    </div>
</template>
<style lang="stylus" scoped>
    .footer-container{
        position: fixed;
        left: 0;
        bottom: 0;
        width: 100%;
        padding: 14px 10px 8px;
        background-color: #fff;
        box-sizing: border-box;
        ul{
            
            height: 2rem;
            border: 1px solid #ccc;
            border-radius: 3px;
            padding: 6px 4px;
            box-sizing: border-box;
            display: flex;
            li{
                flex: 2;
                text-align: center;
                i{
                    vertical-align: middle;
                    margin-right: 4px;
                    color: #666;
                }
                .icon-weather{
                    color: #FA9D26;
                }
            }
            .car-position{
                flex: 4;
                text-align: left;
                overflow: hidden;
                text-overflow: ellipsis;
                display: -webkit-box;
                -webkit-line-clamp: 1;
                -webkit-box-orient: vertical;
            }
            li:last-child{
                border-left: 1px solid #ccc;
            }
        }
    }
</style>