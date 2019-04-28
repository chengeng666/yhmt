<template>
  <div class="container search-container">
    <img class="logo" :src="Logo" />
    <Search />
  </div>
</template>
<script>
import Logo from 'static/images/logo.png'
import Search from './Search'
export default {
  data () {
    return {
      Logo: Logo
    }
  },
  components: {
    Search
  }
}
</script>
<style>
  .search-container {
    height: 130px;
    line-height: 130px;
    vertical-align: middle;
  }
  .logo {
    vertical-align: middle;
    margin-right: 185px;
  }
  @media (max-width: 992px) {
    .search-container {
      text-align: center;
    }
    .logo {
      display: none;
    }
  }
</style>
