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
    <div class="menus">
      <ul class="home-menu">
        <li>
          <nuxt-link to="/home/pay">
            <i class="iconfont">&#xe655;</i>
            <p>自助交费</p>
          </nuxt-link>
        </li>
        <li>
          <nuxt-link to="/home/pay">
            <i class="iconfont">&#xe603;</i>
            <p>预约车位</p>
          </nuxt-link>
        </li>
        <li>
          <nuxt-link to="/home/pay">
            <i class="iconfont">&#xe60f;</i>
            <p>共享车位</p>
          </nuxt-link>
        </li>
      </ul>
      <ul class="home-menu">
        <li>
          <nuxt-link to="/home/pay">
            <i class="iconfont">&#xe679;</i>
            <p>寻找爱车</p>
          </nuxt-link>
        </li>
        <li>
          <nuxt-link to="/home/pay">
            <i class="iconfont">&#xe602;</i>
            <p>附近</p>
          </nuxt-link>
        </li>
        <li>
          <nuxt-link to="/home/pay">
            <i class="iconfont">&#xe676;</i>
            <p>停车记录</p>
          </nuxt-link>
        </li>
      </ul>
      <ul class="home-menu">
        <li>
          <nuxt-link to="/home/pay">
            <i class="iconfont">&#xe603;</i>
            <p>预约记录</p>
          </nuxt-link>
        </li>
        <li>
          <nuxt-link to="/home/pay">
            <i class="iconfont">&#xe620;</i>
            <p>车辆管理</p>
          </nuxt-link>
        </li>
        <li>
          <nuxt-link to="/home/pay">
            <i class="iconfont">&#xe61d;</i>
            <p>停车券</p>
          </nuxt-link>
        </li>
      </ul>
      <ul class="home-menu">
        <li>
          <nuxt-link to="/home/pay">
            <i class="iconfont">&#xe601;</i>
            <p>个人中心</p>
          </nuxt-link>
        </li>
        <li>
          <nuxt-link to="/home/pay">
            <i class="iconfont">&#xe600;</i>
            <p>消息中心</p>
          </nuxt-link>
        </li>
        <li></li>
      </ul>
      <!--<nuxt-link to="/home/pay">自助交费</nuxt-link>
      <nuxt-link to="/home/appoint">预约车位</nuxt-link>-->
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
  .menus{
    margin-top: 8px;
    background-color: #fff;
    margin-bottom: 54px;
  }
  .home-menu{
    display: flex;
    align-content center;
    border-bottom: 1px solid #ccc;
    li{
      flex: 1;
      padding: 40px 20px;
      text-align: center;
      i{
        font-size: 30px;
        color: #FA9D26;
      }
      p{
        margin-top: 4px;
      }
    }
    li + li{
      border-left: 1px solid #ccc;
    }
  }
</style>
