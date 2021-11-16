<template>
  <!--首页头部-->
  <header class="msite_header">
    <slot name="left"></slot>
    <span class="header_title">
      <span class="header_title_text ellipsis">{{ title }}</span>
    </span>
    <slot name="right"></slot>
  </header>
</template>

<script>
export default {
  props: {
    title: String,
  },
};
</script>

<style lang="less" scoped>
.msite_header {
  position: relative;
  top: 0;
  left: 0;
  width: 100%;
  height: 45px;
  background-color: #02a774;
  z-index: 100;
  .header_search {
    position: absolute;
    left: 15px;
    top: 50%;
    transform: translateY(-50%);
    width: 10%;
    height: 50%;
    .icon-sousuo {
      font-size: 25px;
      color: #fff;
    }
  }
  .header_title {
    flex: 1;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 50%;
    color: #fff;
    text-align: center;
    .header_title_text {
      font-size: 20px;
      color: #fff;
      display: block;
    }
  }
  .header_login {
    font-size: 14px;
    color: #fff;
    position: absolute;
    top: 50%;
    right: 15px;
    transform: translateY(-50%);
    .header_login_text {
      color: #fff;
    }
  }
}
</style>