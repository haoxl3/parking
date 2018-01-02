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
          <nuxt-link to="/home/appoint">
            <i class="iconfont">&#xe603;</i>
            <p>预约车位</p>
          </nuxt-link>
        </li>
        <li>
          <nuxt-link to="/home/share">
            <i class="iconfont">&#xe60f;</i>
            <p>共享车位</p>
          </nuxt-link>
        </li>
        <li>
          <nuxt-link to="/home/looking">
            <i class="iconfont">&#xe679;</i>
            <p>寻找爱车</p>
          </nuxt-link>
        </li>
        <li>
          <nuxt-link to="/home/near">
            <i class="iconfont">&#xe602;</i>
            <p>附近</p>
          </nuxt-link>
        </li>
        <li>
          <nuxt-link to="/home/parking">
            <i class="iconfont">&#xe676;</i>
            <p>停车记录</p>
          </nuxt-link>
        </li>
        <li>
          <nuxt-link to="/home/appRecord">
            <i class="iconfont">&#xe603;</i>
            <p>预约记录</p>
          </nuxt-link>
        </li>
        <li>
          <nuxt-link to="/home/carManage">
            <i class="iconfont">&#xe620;</i>
            <p>车辆管理</p>
          </nuxt-link>
        </li>
        <li>
          <nuxt-link to="/home/parkingTicket">
            <i class="iconfont">&#xe61d;</i>
            <p>停车券</p>
          </nuxt-link>
        </li>
        <li>
          <nuxt-link to="/home/personal">
            <i class="iconfont">&#xe601;</i>
            <p>个人中心</p>
          </nuxt-link>
        </li>
        <li>
          <nuxt-link to="/home/messages">
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
    border-bottom: 8px solid #eee;
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
    background-color: #fff;
    margin-bottom: 54px;
  }
  .home-menu{
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-column-gap: 1px;
    grid-row-gap: 1px;
    background-color: #eee;
    li{
      display: flex;
      background-color: #fff;
      justify-content: center;
      align-items: center;
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
      border-left: 1px solid #eee;
    }
  }
</style>
