<template>
  <div class="msite">
    <!-- 首页头部 -->
    <HeaderTop title="武汉理工大学余家头校区">
      <span class="header_search" slot="left">
        <i class="iconfont icon-icon-"></i>
      </span>
      <span class="header_login" slot="right">
         <span class="header_login_text">登陆|注册</span>
      </span>
    </HeaderTop>
    <!-- 首页导航 -->
    <nav class="msite_nav border-1px">
      <div class="swiper-container">
        <div class="swiper-wrapper">
          <div class="swiper-slide">    
              <a href="javascript:" class="link_to_food">
                <div class="food_container">
                  <img  src="../images/nav/1.jpg" alt="">
                </div>
                <span>甜品饮料</span>
              </a>
              <a href="javascript:" class="link_to_food">
                <div class="food_container">
                  <img src="../images/nav/2.jpg" alt="">
                </div>
                <span>美食</span>
              </a>
              <a href="javascript:" class="link_to_food">
                <div class="food_container">
                  <img src="../images/nav/3.jpg" alt="">
                </div>
                <span>药品</span>
              </a>
              <a href="javascript:" class="link_to_food">
                <div class="food_container">
                  <img src="../images/nav/4.jpg" alt="">
                </div>
                <span>超市便利</span>
              </a>
              <a href="javascript:" class="link_to_food">
                <div class="food_container">
                  <img src="../images/nav/5.jpg" alt="">
                </div>
                <span>简餐</span>
              </a>
              <a href="javascript:" class="link_to_food">
                <div class="food_container">
                  <img src="../images/nav/6.jpg" alt="">
                </div>
                <span>准时达</span>
              </a>
              <a href="javascript:" class="link_to_food">
                <div class="food_container">
                  <img src="../images/nav/7.jpg" alt="">
                </div>
                <span>预定早餐</span>
              </a>
              <a href="javascript:" class="link_to_food">
                <div class="food_container">
                  <img src="../images/nav/8.jpg" alt="">
                </div>
                <span>土豪推荐</span>
              </a>
          </div>
          <div class="swiper-slide">
            <a href="javascript:" class="link_to_food">
                <div class="food_container">
                  <img src="../images/nav/9.jpg" alt="">
                </div>
                <span>午餐推荐</span>
              </a>
              <a href="javascript:" class="link_to_food">
                <div class="food_container">
                  <img src="../images/nav/10.jpg" alt="">
                </div>
                <span>晚餐推荐</span>
              </a>
              <a href="javascript:" class="link_to_food">
                <div class="food_container">
                  <img src="../images/nav/11.jpg" alt="">
                </div>
                <span>面食榜单</span>
              </a>
              <a href="javascript:" class="link_to_food">
                <div class="food_container">
                  <img src="../images/nav/12.jpg" alt="">
                </div>
                <span>新店特惠</span>
              </a> 
          </div>
        </div>
        <!-- 分页器 -->
        <div class="swiper-pagination" slot="pagination"></div>
      </div>
    </nav>
    <!-- 首页附近商家 -->
    <div class="msite_shop_list">
      <div class="shop_header">
        <i class="iconfont icon-xuanxiang"></i>
        <span class="shop_header_title">附近商家</span>
      </div>
      <ShopList></ShopList>
    </div>
  </div>
</template>

<script>
import HeaderTop from '../../components/HeaderTop/HeaderTop'
import ShopList from '../../components/ShopList/ShopList'
import Swiper from 'swiper'
import 'swiper/css/swiper.css'

export default {
  mounted(){
    //创建一个swiper实例对象，实现轮播
    new Swiper('.swiper-container',{
      loop: true, // 循环模式选项

      // 如果需要分页器
      pagination: {
        el: '.swiper-pagination',
        clickable:true
      }
    })
  },
  components:{
    HeaderTop,
    ShopList
  }
}
</script>

<style lang="stylus" rel="stylesheet/stylus">
@import "../../common/stylus/mixins.styl" 
  .msite
    .header_search
      flex 2
      text-align left 
      .icon-icon-
        padding-left 15px
        font-size 25px
        color #fff
    .header_login
      flex 2
      text-align center
      font-size 14px
    .msite_nav
      bottom-border-1px(#e4e4e4)
      width 100%
      height 200px
      background #fff
      .swiper-container 
        width: 100%;
        height: 200px;
        .link_to_food
          display inline-block
          width 25%
          margin-top 10px
          margin-left -4px
          .food_container
            display block
            width 100%
            text-align center
            padding-bottom 10px
            font-size 0
            img
              display inline-block
              width 50px
              height 50px
          span 
            display block
            width 100%
            text-align center
            font-size 13px
            color #666
    .msite_shop_list
      top-border-1px(#e4e4e4) 
      margin-top 10px
      background-color #fff 
      .shop_header
        padding 10px 10px 0 10px
        .icon-xuanxiang
          margin-left 5px
          color #999
        .shop_header_title
          color #999
          font-size 14px
          line-height 20px
           

</style>