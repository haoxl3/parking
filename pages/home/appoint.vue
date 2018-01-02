<template>
  <div>
    <m-header><span>预约车位</span></m-header>
    <search></search>
    <div class="parking-containter">
      <park-space-info></park-space-info>
    </div>
    <p class="more">查看附近停车场<i class="iconfont">&#xe609;</i></p>
  </div>
</template>
<script>
import mHeader from '~/components/mHeader.vue'
import search from '~/components/search.vue'
import parkSpaceInfo from '~/components/parkSpaceInfo'

export default {
  methods: {
    goDetail(id) {

    }
  },
  components: {
    mHeader,
    search,
    parkSpaceInfo
  }
}
</script>
<style lang="stylus" scoped>
body{
  background-color: #eee;
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