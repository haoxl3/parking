<template>
  <div>
    <m-header><span>附近</span></m-header>
    <div class="map"></div>
    <div class="near-info-box">
      <park-space-info></park-space-info>
      <park-space-info></park-space-info>
    </div>
  </div>
</template>
<script>
import mHeader from '~/components/mHeader'
import parkSpaceInfo from '~/components/parkSpaceInfo'

export default {
  components: {
    mHeader,
    parkSpaceInfo
  }
}
</script>
<style lang="stylus">
.map{
  height: 200px;
  background-color: pink;
}
.near-info-box{
  background-color: #fff;
}
</style>