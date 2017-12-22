<template>
  <div>
    <m-header :isReturn="false"></m-header>
    <section class="top-banner">
      <div class="avatar-box">
        <div class="avatar"><i class="iconfont"></i></div>
        <p>安然</p>
      </div>
      <i class="iconfont setting">&#xe615;</i>
    </section>
    <div>
      <nuxt-link to="/home/pay">自助交费</nuxt-link>
      <nuxt-link to="/home/appoint">预约车位</nuxt-link>
    </div>
    <m-footer></m-footer>
  </div> 
</template>

<script>
import mHeader from '~/components/mHeader.vue'
import mFooter from '~/components/mFooter.vue'

export default {
  components: {
    mHeader,
    mFooter
  }
}
</script>

<style lang="stylus" scoped>
.top-banner{
  height: 8rem;
  background-color: #fff;
  margin-bottom: 8px;
  position: relative;
  .avatar-box{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    .avatar{
      width: 4rem;
      height: 4rem;
      text-align: center;
      border: 1px solid #eee;
      border-radius: 50%;
      background: url('~/static/imgs/avatar.jpeg') no-repeat center center;
      background-size: cover;
    }
    p{
      text-align: center;
      color: #666;
      margin-top: 0.6rem;
    }
  }
  .setting{
    font-size: 1.4rem;
    position: absolute;
    top: 10px;
    right: 10px;
    color: #888;
  }
}
</style>
