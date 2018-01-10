<template>
  <div>
    <m-header><span>寻找爱车</span></m-header>
    <div class="looking-container">
      <pay-fee></pay-fee>
      <div class="btn" @click="lookingCar" v-show="carFlag">寻车</div>
    </div>
    <div v-show="!carFlag">
      <div class="looking-space">
        <car-pay-info></car-pay-info>
        <p>您的爱车停放位置已在下图中标出，请按照图中所示路线到达停放位置，如遇到问题请拨打寻车热线<span> 400-000-000</span></p>
        <p class="instructions"><i class="iconfont">&#xe605;</i>您当前所在的位置，<i class="iconfont">&#xe602;</i>爱车停放位置</p>
      </div>
      <div class="map"></div>
    </div>
  </div>
</template>
<script>
import mHeader from '~/components/mHeader'
import payFee from '~/components/payFee'
import carPayInfo from '~/components/carPayInfo'

export default {
  data(){
    return{
      carFlag: true
    }
  },
  methods: {
    lookingCar(){
      this.carFlag = false
    }
  },
  components: {
    mHeader,
    payFee,
    carPayInfo
  }
}
</script>
<style lang="stylus">
body{
  background-color: #fff;
}
.looking-container{
  padding: 20px 10px;
  .btn{
    width: 100%;
    margin: 0 auto;
    background-color: #FA9D26;
    padding: 8px 0;
    border-radius: 20px;
    text-align: center;
    color: #fff;
    font-size: 14px;
  }
}
.looking-space{
  padding: 0 10px 10px;
  border-top: 8px solid #eee;
  p{
    line-height: 20px;
    font-size: 14px;
    color: #666;
    span{
      color: #FA9D26;
    }
    i{
      color: #FA9D26;
    }
  }
  .instructions{
    margin-top: 4px;
  }
}
.map{
  height: 200px;
  border-top: 8px solid #eee;
}
</style>