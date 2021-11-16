<template>
  <div class="footer_guide">
    <router-link
      href="javascript:;"
      class="guide_item"
      :to="{ path: '/msite' }"
      active-class="on"
      @click="goTo('/msite')"
    >
      <span class="item_icon">
        <i class="iconfont icon-waimai">&#xe615;</i>
      </span>
      <span>外卖</span>
    </router-link>
    <router-link
      href="javascript:;"
      class="guide_item"
      :to="{ path: '/order' }"
      active-class="on"
      @click="goTo('/order')"
    >
      <span class="item_icon">
        <i class="iconfont icon-search">&#xe634;</i>
      </span>
      <span>搜索</span>
    </router-link>
    <router-link
      href="javascript:;"
      class="guide_item"
      :to="{ path: '/profile' }"
      active-class="on"
      @click="goTo('/profile')"
    >
      <span class="item_icon">
        <i class="iconfont icon-dingdan">&#xe619;</i>
      </span>
      <span>订单</span>
    </router-link>
    <router-link
      href="javascript:;"
      class="guide_item"
      :to="{ path: '/search' }"
      active-class="on"
      @click="goTo('/search')"
    >
      <span class="item_icon">
        <i class="iconfont icon-geren">&#xe608;</i>
      </span>
      <span>我的</span>
    </router-link>
  </div>
</template>

<script>
export default {};
</script>

<style lang="less" scoped>
.icon-waimai::before {
  content: "";
}
.footer_guide {
  border-top: 1px solid #e4e4e4;
  position: fixed;
  z-index: 100;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: #fff;
  width: 100%;
  height: 50px;
  display: flex;
  .guide_item {
    display: flex;
    flex: 1;
    text-align: center;
    flex-direction: column;
    align-items: center;
    margin: 5px;
    color: #999999;
    &.on {
      color: #02a774;
    }
    span {
      font-size: 12px;
      margin-top: 2px;
      margin-bottom: 2px;
      .iconfont {
        font-size: 20px;
      }
    }
  }
}
</style>