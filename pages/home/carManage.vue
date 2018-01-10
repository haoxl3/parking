<template>
    <div>
      <m-header><span>车辆管理</span></m-header>
      <div class="car-container">
        <div class="car-box">
          <ul class="car-item">
            <li>
              <h2>京QC2L85</h2>
              <p>道奇酷威</p>
              <p>发动机号：565846544862214565</p>
            </li>
            <li class="car-img"></li>
          </ul>
        </div>
        <div class="add-car">
          <span><i class="iconfont">&#xe60d;</i></span>
          添加车辆
        </div>
      </div>
    </div>
</template>
<script>
import mHeader from '~/components/mHeader.vue'
export default {
  components: {
    mHeader
  }
}
</script>
<style lang="stylus">
body{
  background-color: #eee;
}
.car-container{
  background-color: #fff;
  .car-box{
    border-bottom: 1px solid #eee;
  }
  .car-item{
    display: flex;
    li{
      padding: 20px 10px;
      border-bottom: 1px solid #ccc;
      h2{
        font-size: 20px;
        color: #FA9D26;
      }
      p{
        margin-top: 10px;
        font-size: 14px;
      }
    }
    .car-img{
      background: url('~/static/imgs/car.png') no-repeat center center;
      background-size: contain;
    }
    li:first-child{
      flex: 2;
    }
    li:last-child{
      flex: 1;
    }
  }
  .add-car{
    padding: 20px 0;
    text-align: center;
    font-size: 16px;
    span{
      width: 40px;
      height: 40px;
      line-height: 40px;
      display: inline-block;
      border: 1px dotted #333;
      border-radius: 8px;
      text-align: center;
      vertical-align: middle;
      margin-right: 4px;
    }
    i{
      font-size: 24px;
    }
  }
}
</style>