<template>
  <div>
    <m-header><span>自助交费</span></m-header>
    <div class="container">
      <pay-fee></pay-fee>
      <div class="long-btn">查询</div>
    </div>
    <div class="item-container">
      <park-info></park-info>
    </div>
    <p class="more">查看更多停车记录<i class="iconfont">&#xe609;</i></p>
  </div> 
</template>
<script>
import mHeader from '~/components/mHeader.vue'
import payFee from '~/components/payFee.vue'
import parkInfo from '~/components/parkInfo.vue'
export default {
  components: {
    mHeader,
    payFee,
    parkInfo
  }
}
</script>
<style lang="stylus" scoped>
body{
  background-color: #eee;
}
.container{
  padding: 10px;
  background-color: #fff;
}
.item-container{
  background-color: #fff;
}
.more{
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