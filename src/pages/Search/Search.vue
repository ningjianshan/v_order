<template>
  <section class="profile">
    <HeaderTop title="我的"></HeaderTop>
    <section class="profile-number">
      <router-link href="javascript:" class="profile-link" to="/login">
        <div class="profile_image">
          <i class="iconfont icon-person">&#xe608;</i>
        </div>
        <div class="user-info">
          <p class="user-info-top">登录/注册</p>
          <p>
            <span class="user-icon">
              <i class="iconfont icon-shouji icon-mobile"></i>
            </span>
            <span class="icon-mobile-number">暂无绑定手机号</span>
          </p>
        </div>
        <span class="arrow">
          <i class="iconfont icon-jiantou1">&#xe65f;</i>
        </span>
      </router-link>
    </section>
    <section class="profile_info_data border-1px">
      <ul class="info_data_list">
        <a href="javascript:" class="info_data_link">
          <span class="info_data_top"><span>0.00</span>元</span>
          <span class="info_data_bottom">我的余额</span>
        </a>
        <a href="javascript:" class="info_data_link">
          <span class="info_data_top"><span>0</span>个</span>
          <span class="info_data_bottom">我的优惠</span>
        </a>
        <a href="javascript:" class="info_data_link">
          <span class="info_data_top"><span>0</span>分</span>
          <span class="info_data_bottom">我的积分</span>
        </a>
      </ul>
    </section>
    <section class="profile_my_order border-1px">
      <!-- 我的订单 -->
      <a href="javascript:" class="my_order">
        <span>
          <i class="iconfont icon-order-s">&#xe787;</i>
        </span>
        <div class="my_order_div">
          <p>我的订单</p>
          <span class="my_order_icon">
            <i class="iconfont icon-jiantou1">&#xe65f;</i>
          </span>
        </div>
      </a>
      <!-- 积分商城 -->
      <a href="javascript:" class="my_order">
        <span>
          <i class="iconfont icon-jifen">&#xe686;</i>
        </span>
        <div class="my_order_div">
          <p>积分商城</p>
          <span class="my_order_icon">
            <i class="iconfont icon-jiantou1">&#xe65f;</i>
          </span>
        </div>
      </a>
      <!-- 硅谷外卖会员卡 -->
      <a href="javascript:" class="my_order">
        <span>
          <i class="iconfont icon-vip">&#xe886;</i>
        </span>
        <div class="my_order_div">
          <p>硅谷外卖会员卡</p>
          <span class="my_order_icon">
            <i class="iconfont icon-jiantou1">&#xe65f;</i>
          </span>
        </div>
      </a>
    </section>
    <section class="profile_my_order border-1px">
      <!-- 服务中心 -->
      <a href="javascript:" class="my_order">
        <span>
          <i class="iconfont icon-fuwu">&#xe60c;</i>
        </span>
        <div class="my_order_div">
          <p>服务中心</p>
          <span class="my_order_icon">
            <i class="iconfont icon-jiantou1">&#xe65f;</i>
          </span>
        </div>
      </a>
    </section>
  </section>
</template>

<script>
import HeaderTop from "../../components/HeaderTop/HeaderTop.vue";
export default {
  components: {
    HeaderTop,
  },
};
</script>

<style lang="less" scoped>
.profile {
  width: 100%;
  .profile-number {
    border-top: 1px solid #fff;
    .profile-link {
      position: relative;
      display: block;
      background: #02a774;
      padding: 20px 10px;
      &::after {
        content: "";
        display: block;
        clear: both;
      }
      .profile_image {
        float: left;
        width: 60px;
        height: 60px;
        border-radius: 50%;
        overflow: hidden;
        vertical-align: top;
        .icon-person {
          background: #e4e4e4;
          font-size: 62px;
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
            height: 20px;
            .icon-mobile {
              font-size: 25px;
              vertical-align: text-top;
            }
          }
          .icon-mobile-number {
            font-size: 14px;
            color: #fff;
          }
        }
      }
      .arrow {
        width: 12px;
        height: 12px;
        position: absolute;
        right: 15px;
        top: 40%;
        .icon-jiantou1 {
          color: #fff;
          font-size: 15px;
        }
      }
    }
  }
  .profile_info_data {
    position: relative;
    width: 100%;
    background: #fff;
    overflow: hidden;
    &::before {
      content: "";
      position: absolute;
      z-index: 200;
      left: 0;
      bottom: 0;
      width: 100%;
      height: 1px;
      background-color: #e4e4e4;
      transform: scaleY(0.5);
    }
    .info_data_list {
      &::after {
        content: "";
        display: block;
        clear: both;
      }
      .info_data_link {
        float: left;
        width: 33%;
        text-align: center;
        border-right: 1px solid #f1f1f1;
        .info_data_top {
          display: block;
          width: 100%;
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
        .info_data_top {
          span {
            color: #6ac20b;
          }
        }
      }
    }
  }
  .profile_my_order {
    position: relative;
    margin-top: 10px;
    background: #fff;
    .my_order {
      display: flex;
      align-items: center;
      padding-left: 15px;
      &::before {
        content: "";
        position: absolute;
        z-index: 200;
        left: 0;
        top: 0;
        width: 100%;
        height: 1px;
        background-color: #e4e4e4;
      }
      span {
        display: flex;
        align-items: center;
        width: 20px;
        height: 20px;
        .iconfont {
          margin-left: -10px;
          font-size: 25px;
        }
        .icon-order-s {
          color: #02a774;
        }
        .icon-jifen {
          color: #ff5f3e;
        }
        .icon-vip {
          color: #f90;
        }
        .icon-fuwu {
          color: #02a774;
        }
      }
      .my_order_div {
        width: 100%;
        border-bottom: 1px solid #f1f1f1;
        padding: 18px 10px 18px 0;
        font-size: 16px;
        color: #333;
        display: flex;
        justify-content: space-between;
        p {
          display: block;
        }
        .my_order_icon {
          width: 10px;
          height: 10px;
          .icon-jiantou1 {
            color: #bbb;
            font-size: 10px;
          }
        }
      }
    }
  }
}
</style>