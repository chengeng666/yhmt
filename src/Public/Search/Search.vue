<template>
  <div class="search-box">
    <div class="search">
      <input class="search-input" type="text"/>
      <a class="search-btn">搜索</a>
    </div>
    <div class="search-text">
      <a>香奈儿</a>
      <span>|</span>
      <a>奶粉</a>
      <span>|</span>
      <a>家具</a>
    </div>
  </div>
</template>
<script>
export default {
}
</script>
<!--scoped  样式私有化  只有这个组件会读取到里面的样式-->
<style scoped>
  .search-box {
    width: 428px;
    display: inline-block;
    line-height: normal;
    vertical-align: middle;
  }
  .search {
    position: relative;
    width: 100%;
    height: 42px;
    border: 2px solid #ff2d52;
  }
  .search-input {
    width: 100%;
    height: 100%;
    line-height: 38px;
    border: 0;
    padding-left: 30px;
    color: #aaa;
    font-size: 14px;
    background: url("../image/icon-search.png") no-repeat 8px center;
  }
  .search-input:focus {
    outline: none;
  }
  .search-btn {
    width: 78px;
    height: 38px;
    display: inline-block;
    background: #ff2d52;
    text-align: center;
    line-height: 38px;
    font-size: 16px;
    color: #fff;
    position: absolute;
    right: 0;
    top: 0;
  }

  /*搜索文本*/
  .search-text {
    margin-top: 8px;
    color: #333;
  }
  @media (max-width: 748px) {
    .search-box {
      max-width: 100%;
      text-align: left;
    }
    .search {
      -webkit-border-radius: 25px;
      -moz-border-radius: 25px;
      border-radius: 25px;
      overflow: hidden;
    }
  }

</style>
