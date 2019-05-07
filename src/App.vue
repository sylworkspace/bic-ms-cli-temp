<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<style lang="less">
@import url('./assets/style/index.css');
#app {
  height: 100%;
  .bic {
    height: 100%;
    .bic-header {
      width: 100%;
      background: #fff;
      .bic-header-log {
        width: 200px;
        float: left;
        text-align: center;
        height: 61px;
        line-height: 60px;
      }
      .bic-header-list {
        width: calc(100% - 200px);
        float: left;
      }
      &:after {
        content: '';
        display: block;
        clear: both;
      }
    }
    .bic-main {
      width: 100%;
      height: 100%;
      .bic-main-list {
        width: 200px;
        height: 100%;
        background: #fff;
        border-right: solid 1px #e6e6e6;
        float: left;
      }
      .bic-main-list-min-width {
        width: 64px;
      }
      .bic-main-list-mmax-width {
        width: 200px;
      }
      .bic-main-content {
        width: 100%;
        height: 100%;
        box-sizing: border-box;
        .bic-main-content-crumb {
          span {
            font-size: 14px;
            color: #909399
          }
          padding-left: 20px;
          width: 100%;
          height: 50px;
          line-height: 50px;
          box-sizing: border-box;
          background: #fff;
        }
        .bic-main-content-content {
          width: 100%;
          height: 100%;
        }
      }
      .bic-main-content-padding-small {
        padding-left: 63px;
      }
      .bic-main-content-padding-lager {
        padding-left: 200px;
      }
    }
  }
}
</style>
