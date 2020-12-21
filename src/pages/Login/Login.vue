<template>
  <div class="login_container">
      <div class="login_inner">
        <div class="login_header">
            <h2 class="login_title">武理订餐</h2>
        </div>
        <div class="login_content">
            <form action="">
                <section class="login_telnumber">
                    <input type="text" maxlength="10" placeholder="手机号">
                    <button class="get_verification">获取验证码</button>
                </section>
                <section class="login_vertification">
                    <input type="password" placeholder="验证码">
                </section>
                <section class="login_tip">
                    温馨提示：未注册武理订餐应用的手机号，登录时将自动注册，且代表已同意
                    <a href="javascript:;">《用户服务协议》</a>
                </section>
                <button class="login_submit">登录</button>
            </form>
            <a href="javascript:;" class="about_us">关于我们</a>
        </div>
        <span class="go_back" @click="$router.back()">
            <i class="iconfont icon-xiazai6"></i>
        </span>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="stylus" rel="stylesheet/stylus">
  .login_container
    background-color #fff
    position relative
    .go_back
      position absolute
      top 5px
      left 5px
      color #ccc
    .login_inner
      padding-top 60px
      width 80%
      margin 0 auto
      .login_header
        font-size 40px
        font-weight 700
        color #02a774
        text-align center
      .login_content
        >form
          input 
            width 100%
            height 100%
            padding-left 10px
            box-sizing border-box
            border 1px solid #ddd
            border-radius 4px
            font 400 14px Arial
            &:focus
              border 1px solid #02a774
          .login_telnumber
            position relative
            margin-top 50px
            height 48px
            font-size 14px
            .get_verification
              position absolute
              top 50%
              right 10px
              transform translateY(-50%)
              border 0
              color #cccccc
              font-size 14px
              background transparent
          .login_vertification
            margin-top 16px
            height 48px
            font-size 14px
          .login_tip
            margin-top 15px
            font-size 14px
            color #807e7e
            >a
              color #02a774
          .login_submit
            display block
            width 100%
            height 42px
            margin-top 30px
            border-radius 4px
            background #4cd96f
            color #ffffff
            text-align center
            font-size 16px
            line-height 42px
            border 0
        .about_us
          display block
          width 50%
          margin 15px auto
          text-align center



            
            
        
</style>