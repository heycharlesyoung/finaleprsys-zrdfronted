<template>
    <el-container class="home-container">
        <!-- 头部 -->
        
    <el-header class="el-header">
        <div>
            <img src="" alt="">
            <span>招生宣传报名系统</span>
        
        </div>
        <el-button type="info" @click="logout">退出</el-button>
        
    </el-header>
    <el-container>
      <!-- 侧边栏 -->
    <el-aside width="200px" class="el-aside">
        <el-menu
      
      background-color="#545c64"
      text-color="#fff"
      active-text-color="#ffd04b">
      <!-- 一级菜单 -->
      <el-submenu index="1">
          <!-- 一级菜单模板区域 -->
        <template slot="title">
            <!-- 图标 -->
          <i class="el-icon-location"></i>
          <!-- 文本 -->
          <span>导航一</span>
        </template>
          <!-- 二级菜单 -->
          <el-menu-item index="1-4-1"><template slot="title">
            <!-- 图标 -->
          <i class="el-icon-location"></i>
          <!-- 文本 -->
          <span>导航一</span>
        </template></el-menu-item>
      </el-submenu>
    </el-menu>
    </el-aside>
    <!-- 右侧内容主体 -->
    <el-main class="el-main">Main</el-main>
    </el-container>
</el-container>
</template>
<script>
export default {
    methods:{
        logout(){
            window.sessionStorage.clear()
            this.$router.push('/login')
        }
    }
}
</script>
<style lang="less" scoped>
.home-container{
    height:100%;
}
.el-header{
    background-color: #373d41;
    display: flex;
    justify-content: space-between;
    padding-left: 0;
    align-items: center;
    color: #fff;
    font-size: 20px;
    > div{
        display: flex;
        align-items: center;
        span{
            margin-left: 15px;
        }
    }

}
.el-aside{
    background-color: #333744;

}
.el-main{
    background-color: #eaedf1;
}
</style>