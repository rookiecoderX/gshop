<template>
  <div class="profile-container">
    <section class="profile">
      <mt-header fixed title="我的" class="bg"></mt-header>
      <section class="profile-number">
        <router-link to="/login" class="profile-link">
          <div class="profile_image">
            <i class="iconfont iconwodedangxuan"></i>
          </div>
          <div class="user-info">
            <p class="user-info-top">登录/注册</p>
            <p>
              <span class="user-icon">
                <i class="iconfont icon-shouji iconshouji"></i>
              </span>
              <span class="icon-mobile-number">暂无绑定手机号</span>
            </p>
          </div>
          <span class="arrow">
            <i class="iconfont iconarrowRight"></i>
          </span>
        </router-link>
      </section>
      <section class="profile_info_data border-1px">
        <ul class="info_data_list">
          <a href="javascript:" class="info_data_link">
            <span class="info_data_top">
              <span>0.00</span>元
            </span>
            <span class="info_data_bottom">我的余额</span>
          </a>
          <a href="javascript:" class="info_data_link">
            <span class="info_data_top">
              <span>0</span>个
            </span>
            <span class="info_data_bottom">我的优惠</span>
          </a>
          <a href="javascript:" class="info_data_link">
            <span class="info_data_top">
              <span>0</span>分
            </span>
            <span class="info_data_bottom">我的积分</span>
          </a>
        </ul>
      </section>
      <section class="profile_my_order border-1px">
        <!-- 我的订单 -->
        <a href="javascript:" class="my_order">
          <span>
            <i class="iconfont icon6"></i>
          </span>
          <div class="my_order_div">
            <span>我的订单</span>
            <span class="my_order_icon">
              <i class="iconfont iconarrowRight"></i>
            </span>
          </div>
        </a>
        <!-- 积分商城 -->
        <a href="javascript:" class="my_order">
          <span>
            <i class="iconfont icongifts"></i>
          </span>
          <div class="my_order_div">
            <span>积分商城</span>
            <span class="my_order_icon">
              <i class="iconfont iconarrowRight"></i>
            </span>
          </div>
        </a>
        <!-- 硅谷外卖会员卡 -->
        <a href="javascript:" class="my_order">
          <span>
            <i class="iconfont iconhuiyuan"></i>
          </span>
          <div class="my_order_div">
            <span>会员卡</span>
            <span class="my_order_icon">
              <i class="iconfont iconarrowRight"></i>
            </span>
          </div>
        </a>
      </section>
      <section class="profile_my_order border-1px">
        <!-- 服务中心 -->
        <a href="javascript:" class="my_order">
          <span>
            <i class="iconfont iconkefu"></i>
          </span>
          <div class="my_order_div">
            <span>服务中心</span>
            <span class="my_order_icon">
              <i class="iconfont iconarrowRight"></i>
            </span>
          </div>
        </a>
      </section>
    </section>
  </div>
</template>
<script>
export default {

}
</script>
<style lang='less' scoped>
@import '../../common/less/mixin.less';
.profile-container {
  .profile {
    .profile-number {
      margin-top: 41px;
      .profile-link {
        .clearfix();
        position: relative;
        display: block;
        background-color: #02a774;
        padding: 20px 10px;
        .profile_image {
          float: left;
          width: 60px;
          height: 60px;
          border-radius: 50%;
          overflow: hidden;
          vertical-align: top;
          .iconwodedangxuan {
            background-color: #e4e4e4;
            font-size: 62px;
            color: #ccc;
          }
        }
        .user-info {
          float: left;
          margin-top: 8px;
          margin-left: 15px;
          p {
            font-weight: 700;
            font-size: 18px;
            color: #fff;
            &.user-info-top {
              padding-bottom: 8px;
            }
            .user-icon {
              display: inline-block;
              margin-left: -15px;
              margin-right: 5px;
              width: 20px;
              height: 2px;
              .iconshouji {
                margin-left: 10px;
                font-size: 20px;
                vertical-align: center;
              }
            }
            .icon-mobile-number {
              font-size: 14px;
              color: #fff;
            }
          }
        }
        .arrow {
          position: absolute;
          width: 12px;
          height: 12px;
          right: 15px;
          top: 40%;
          .iconarrowRight {
            color: #fff;
            font-size: 5px;
          }
        }
      }
    }
    .profile_info_data {
      .bottom-border-1px(#e4e4e4);
      width: 100%;
      background-color: #fff;
      overflow: hidden;
      .info_data_list {
        .clearfix();
        .info_data_link {
          float: left;
          width: 33%;
          text-align: center;
          border-right: 1px solid #f1f1f1;
          .info_data_top {
            display: block;
            width: 100px;
            font-size: 14px;
            color: #333;
            padding: 15px 5px 10px;
            span {
              display: inline-block;
              font-size: 30px;
              color: #f90;
              font-weight: 700;
              line-height: 30px;
            }
          }
          .info_data_bottom {
            display: inline-block;
            font-size: 14px;
            color: #666;
            font-weight: 400;
            padding-bottom: 10px;
          }
        }
        .info_data_link:nth-of-type(2) {
          .info_data_top {
            span {
              color: #ff5f3e;
            }
          }
        }
        .info_data_link:nth-of-type(3) {
          border: 0;
          .info_data_top {
            span {
              color: #6ac20b;
            }
          }
        }
      }
    }
    .profile_my_order {
      .top-border-1px(#e4e4e4);
      margin-top: 10px;
      background-color: #fff;
      .my_order {
        display: flex;
        align-items: center;
        padding-left: 15px;
        > span {
          display: flex;
          align-items: center;
          width: 20px;
          height: 20px;
          > .iconfont {
            font-size: 20px;
          }
          .icon6 {
            color: #02a774;
          }
          .icongifts {
            color: #ff5f3e;
          }
          .iconhuiyuan {
            color: #f99;
          }
          .iconkefu {
            color: #02a774;
          }
        }
        .my_order_div {
          width: 100%;
          border-bottom: 1px solid #f1f1f1;
          padding: 18px 10px 18px 10px;
          font-size: 16px;
          color: #333;
          display: flex;
          justify-content: space-between;
          span {
            display: block;
          }
          .my_order_icon {
            width: 10px;
            height: 10px;
            .iconarrowRight {
              color: #bbb;
              font-size: 10px;
            }
          }
        }
      }
    }
  }
}
</style>
