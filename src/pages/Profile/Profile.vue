<template>
  <section class="profile">
    <HeaderTop title="我的"></HeaderTop>
    <section class="profile-number">
      <router-link to="/login" class="profile-link">
        <div class="left">
          <div class="profile_image">
          <i class="iconfont icon-geren"></i>
        </div>
        </div>
        <div class="user-info">
          <p class="user-info-top">登陆/注册</p>
          <p class="user-phone">
            <span class="user-icon">
              <i class="iconfont icon-phone"></i>
            </span>
            <span class="icon-mobile-number">暂无手机号绑定</span>
          </p>
        </div>
        <div class="arrow">
          <i class="iconfont icon-z043"></i>
        </div>
      </router-link>
    </section>
    <section class="profile_info_data" border-1px>
      <ul class="info_data_list">
        <li>
          <a href="javascript:" class="info_data_link">
            <div class="info_data_top"><span>0.00</span>元</div>
            <div class="info_data_bottom">我的余额</div>
          </a>
        </li>
        <li>
          <a href="javascript:" class="info_data_link">
            <div class="info_data_top"><span>0</span>个</div>
            <div class="info_data_bottom">我的优惠</div>
          </a>
        </li>
        <li>
          <a href="javascript:" class="info_data_link">
            <div class="info_data_top"><span>0</span>分</div>
            <div class="info_data_bottom">我的积分</div>
          </a>
        </li>
      </ul>
    </section>
    <section class="profile_my_order border-1px">
      <a href="javascript:" class="my_order">
        <span class="my_order_icon">
          <i class="iconfont icon-icon"></i>
        </span>
        <span class="my_order_span">我的订单</span>
        <span class="jiantou">
          <i class="iconfont icon-z043"></i>
        </span>
      </a>
      <a href="javascript:" class="my_order">
        <span class="my_order_icon">
          <i class="iconfont icon-jifen"></i>
        </span>
        <span class="my_order_span">积分商城</span>
        <span class="jiantou">
          <i class="iconfont icon-z043"></i>
        </span>
      </a>
      <a href="javascript:" class="my_order">
        <span class="my_order_icon">
          <i class="iconfont icon-huiyuan"></i>
        </span>
        <span class="my_order_span">外卖会员卡</span>
        <span class="jiantou">
          <i class="iconfont icon-z043"></i>
        </span>
      </a>
      <a href="javascript:" class="my_order">
        <span class="my_order_icon">
          <i class="iconfont icon-fuwuzhongxin"></i>
        </span>
        <span class="my_order_span">服务中心</span>
        <span class="jiantou">
          <i class="iconfont icon-z043"></i>
        </span>
      </a>
    </section>
  </section>
</template>

<script>
import HeaderTop from '../../components/HeaderTop/HeaderTop'
export default {
  components:{
    HeaderTop
  }
}
</script>

<style lang="stylus" rel="stylesheet/stylus">
@import "../../common/stylus/mixins.styl" 
  .profile
    overflow hidden
    .profile-number
      margin-top 1px
      .profile-link
        display flex
        justify-content center
        justify-items center
        background #02a774
        padding 20px 10px
        .left
          flex 2
          .profile_image
            width 60px
            height 60px
            line-height 67px
            border-radius 50%
            overflow hidden
            background #fff
            text-align center
            .icon-geren
              font-size 65px
              margin-left -2px
        .user-info
          flex 8
          margin 8px 0 0 15px
          color #fff
          text-align left
          .user-info-top
            font-size 18px
            font-weight 700
          .user-phone
            height 20px
            margin-left -5px
            .user-icon
              display inline-block
              width 20px
              .icon-phone
                font-size 20px
            .icon-mobile-number
              margin-left -5px
              font-size 16px
        .arrow
          flex 1
          color #fff
          .icon-z043
            display block
            margin-top 20px
    .profile_info_data
      .info_data_list
        display flex
        li
          flex 1
          padding 10px
          text-align center
          background-color #fff
          &:nth-child(1) 
            border-right 1px solid #666
          &:nth-child(2)
            border-right 1px solid #666
          .info_data_link
          display flex
            flex-direction column
            .info_data_top
              flex 1
              padding-bottom 8px
              span 
                color #efa220
                font-size 25px
                font-weight 700
            .info_data_bottom
              flex 1
    .profile_my_order
      display flex
      flex-direction column
      margin-top 10px
      height 160px 
      .my_order
        display flex
        flex 1
        background-color #fff
        line-height 40px
        font-size 16px
        color #000
        &:nth-child(-n+3)
          bottom-border-1px(#e4e4e4)
        &:last-child
          margin-top 10px
        .my_order_icon
          flex 1
          text-align right 
          padding-right 5px
          .icon-icon
            color #02a774
          .icon-jifen
            color #ff5f3e
          .icon-huiyuan
            color #f90
          .icon-fuwuzhongxin
            color #02a774
        .my_order_span
          flex 10
        .jiantou
          flex 1

        

      
          
      
</style>