<template>
  <div>
    <m-header><span>自助交费</span></m-header>
    <div class="container">
      <pay-fee></pay-fee>
      <div class="long-btn">查询</div>
    </div>
    <div class="item-container">
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
          <li><span class="paied">已交费</span></li>
        </ul>
      </div>
    </div>
    <p class="more-pay">查看更多停车记录<i class="iconfont">&#xe609;</i></p>
  </div> 
</template>
<script>
import mHeader from '~/components/mHeader.vue'
import payFee from '~/components/payFee.vue'
export default {
  components: {
    mHeader,
    payFee
  }
}
</script>
<style lang="stylus">
body{
  background-color: #eee;
}
.container{
  padding: 10px;
  background-color: #fff;
}
.item-container{
  background-color: #fff;
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
}
.more-pay{
  text-align: center;
  color: #2484E0;
  line-height: 30px;
  background-color: #fff;
  i{
    color: #ccc;
    vertical-align: middle;
    margin-left: 6px;
  }
}
</style>