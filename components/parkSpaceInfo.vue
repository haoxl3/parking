<template>
    <div class="item" id="0">
        <div class="flex-left">
            <p class="adress"><i>P</i>燕东大厦停车场</p>
            <ul class="parking-intro clearfix">
            <li>园区</li>
            <li>地面</li>
            <li>现金支付</li>
            <li>免16分钟</li>
            </ul>
            <ul class="parking-info">
            <li>价格：约5.0元/小时</li>
            <li>剩余车位：暂未开通</li>
            </ul>
        </div>
        <div class="flex-right">
            <div class="circle-box">
            <div class="circle">
                <nuxt-link to="/0/appCar"><i class="iconfont">&#xe66d;</i></nuxt-link>
            </div>
            <p>250米</p>
            </div>
        </div>
    </div>
</template>
<style lang="stylus" scoped>
.item{
  background-color: #fff;
  border-bottom: 1px solid #eee;
  padding: 20px 10px;
  display: flex;
  .flex-left{
    flex: 8;
    .adress{
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
    .parking-intro{
      margin-top: 10px;
      li{
        float: left;
        padding: 0 4px;
        border-right: 1px solid #ccc;
        font-size: 14px;
      }
      li:last-child{
        border-right: none;
      }
      li:first-child{
        padding-left: 0;
      }
    }
    .parking-info{
      display: flex;
      margin-top: 10px;
      li{
        flex: 1;
      }
    }
  }
  .flex-right{
    flex: 2;
    position: relative;
    text-align: center;
    .circle-box{
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      p{
        margin-top: 4px;
      }
    }
    .circle{
      width: 50px;
      height: 50px;
      border: 1px solid #ccc;
      border-radius: 50%;
      text-align: center;
      i{
        font-size: 20px;
        color: #FA9D26;
        line-height: 50px;
      }
    }
  }
}
</style>