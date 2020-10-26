<template>
    <div class="nav-bar">
        <nuxt-link to="/" class="logo">刀刀 & Mammon的博客</nuxt-link>
        <nuxt-link to="/articlelist" class="nav-item">
            文章列表
        </nuxt-link>
        <nuxt-link to="/" class="nav-item">
            个人作品
        </nuxt-link>
        <div class="search-place">
            <input class="search" type="text">
            <div class="search-button">
                <nuxt-link to="/search"><icon name="search" scale="4"></icon></nuxt-link>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    methods:{
        
    }
}
</script>

<style lang="scss" scoped>
.nav-bar{
  height:50px;
  position: fixed;
  width:100%;
  box-sizing: border-box;
  background:#91d281;
  padding:0 20px;
  .logo{
      font-size:22px;
      color:#fff;
      line-height:50px;
      text-decoration: none;
      margin-right:80px;
      vertical-align: middle;
  }
  .nav-item{
    color:#fff;
    line-height: 50px;
    text-decoration: none;
    vertical-align: middle;
    padding:0 20px;
    transition: all .3s;
    display: inline-block;
    height:50px;
    position: relative;
    &:before{
        content:'';
        display: block;
        opacity:0;
        position:absolute;
        top:10px;
        left:-10px;
        width:30px;
        height:30px;
        background-image: url("~assets/flower.png");
        background-size: cover;
        z-index:0;
        transition: all 0.3s;
    }
    &:hover{
        &::before{
            opacity:1;
        }
    }
  }
  .search-place{
      float:right;
      height:50px;
      position: relative;
      .search{
          height:40px;
          width:400px;
          margin-top:5px;
          padding:0 20px;
          box-sizing: border-box;
          outline: none;
          border:none;
          font-size:18px;
          color:#666;
          border-radius: 20px;;
      }
      .search-button{
          font-size:20px;
          width:30px;
          height:30px;
          position: absolute;
          top:5px;
          right:10px;
          cursor: pointer;
      }
  }
}
</style>