<template>
  <div class="shop_container">
      <ul class="shop_list">
          <li class="shop_li border-1px">
              <a href="#">
                  <div class="shop_left">
                      <img class="shop_img" src="./images/shop/4.jpg" alt="">
                  </div>
                  <div class="shop_right">
                      <section class="shop_detail_header">
                          <h4 class="shop_title">中快餐厅</h4>
                          <div class="rating_order_section">
                              <div class="start">
                                <span class="star-item on"></span>
                                <span class="star-item on"></span>
                                <span class="star-item on"></span>
                                <span class="star-item on"></span>
                                <span class="star-item off"></span>
                              </div>
                              <span class="rating_span">4.0</span>
                              <span class="order_span">月售106单</span>
                          </div>
                          <div class="send_price">
                            <span>￥20起送/配送费约￥2</span>
                          </div>
                      </section>
                  </div>
              </a>
          </li>
           <li class="shop_li border-1px">
              <a href="#">
                  <div class="shop_left">
                      <img class="shop_img" src="./images/shop/4.jpg" alt="">
                  </div>
                  <div class="shop_right">
                      <section class="shop_detail_header">
                          <h4 class="shop_title">水运一食堂</h4>
                          <div class="rating_order_section">
                              <div class="start">
                                <span class="star-item on"></span>
                                <span class="star-item on"></span>
                                <span class="star-item on"></span>
                                <span class="star-item half"></span>
                                <span class="star-item off"></span>
                              </div>
                              <span class="rating_span">3.6</span>
                              <span class="order_span">月售79单</span>
                          </div>
                          <div class="send_price">
                            <span>￥20起送/配送费约￥2</span>
                          </div>
                      </section>
                  </div>
              </a>
          </li>
      </ul>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="stylus" rel="stylesheet/stylus">
@import "../../common/stylus/mixins.styl" 
  .shop_container
    .shop_list
      .shop_li
        bottom-border-1px(#f1f1f1)
        width 100%
        >a
          clearFix()
          display flex
          justify-content center
          box-sizing border-box
          padding 15px 8px
          width 100%
          .shop_left
            flex 2
            padding-right 10px
            .shop_img
              display block
              width 100%
              height 100%
              padding-right 10px
          .shop_right
            flex 6
            display flex
            flex-direction column
            justify-items center
            .shop_detail_header
              .shop_title
                flex 1
                padding-bottom 10px
                width 200px
                line-height 16px
                font-size 16px
                font-weight 700
                color #000
                text_ellipsis()
                &::before
                  content '品牌'
                  display inline-block
                  font-size 11px
                  line-height 11px
                  color #333
                  background-color #ffd930
                  padding 2px 2px
                  border-radius 2px
                  margin-right 5px
              .rating_order_section
                padding-bottom 10px
                font-size 10px
                flex 1
                .start
                  display inline-block
                .star-item
                  display inline-block
                  width 10px
                  height 10px
                  margin-right 1px
                  background-size 10px 10px
                  &:last-child
                    margin-right: 0
                  &.on
                    bg-image('./images/stars/star24_on')
                  &.half
                    bg-image('./images/stars/star24_half')
                  &.off
                    bg-image('./images/stars/star24_off')
                .rating_span
                  color #ff6000
                  margin-right 5px
                .order_span
                  color #666
              .send_price
                font-size 10px
                flex 1
</style>