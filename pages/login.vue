<template>
    <div class="login-container">
        <m-header :isReturn="false">
            <span>欢迎使用乐亦驾</span>
        </m-header>
        <form class="login-box">
            <ul>
                <li class="phone">中国<span>+86<i></i></span></li>
                <li class="user"><input type="text" placeholder="请输入手机号"/></li>
            </ul>
            <ul>
                <li>短信验证码</li>
                <li><input type="password"/></li>
                <li class="identifying-code-box">
                    <div>获取验证码</div>
                </li>
            </ul>
        </form>
        <div class="login-btn">授权登录</div>
        <p class="service">服务电话：<i>400-500-600</i></p>
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
    background-color: #fff;
}
.login-box{
    margin: 20px 0 30px;
    padding: 0 10px;
    ul{
        display: flex;
        padding: 10px 4px;
        border-top: 1px solid #ccc;
        li{
            flex: 1;
            font-size: 14px;
            input{
                width: 100%;
                height: 100%;
                padding-left: 6px;
                box-sizing: border-box;
            }
        }
        li:first-child{
            width: 130px;
            padding: 10px 4px;
        }
        li:nth-child(2n){
            border-left: 1px solid #ccc;
        }
        li.user{
            flex: 2;
        }
        .identifying-code-box{
            div{
                width: 100%;
                height: 36px;
                line-height: 36px;
                background-color: #FA9D26;
                border-radius: 3px;
                color: #fff;
                font-size: 12px;
                text-align: center;
            }
        }
    }
    ul:last-child{
        border-bottom: 1px solid #ccc;
    }
    .phone{
        position: relative;
        span{
            color: #FA9D26;
            float: right;
            margin-right: 14px;
            i{
                position: absolute;
                right: 4px;
                bottom: 0;
                border: 6px solid #FA9D26;
                border-top: 6px solid transparent;
                border-left: 6px solid transparent;
            }
        }
    }
}
.login-btn{
    width: 80%;
    height: 30px;
    line-height: 30px;
    margin: 0 auto 20px;
    border-radius: 20px;
    background-color: #FA9D26;
    color: #fff;
    text-align: center;
}
.login-container{
    .service{
        text-align: center;
        color: #bbb;
        i{
            color: #FA9D26;
        }
    }
}
</style>