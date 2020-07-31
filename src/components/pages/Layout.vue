<template>
    <div class="wapper">
        <el-container class="container" direction="">
            <el-aside>
                <SideBar></SideBar>
            </el-aside>
            <el-container>
                <el-header>Header <i class="el-icon-warning-outline"></i></el-header>
                <el-main>Main<el-button round><i class="el-icon-search"></i></el-button></el-main>
            </el-container>
        </el-container>
    </div>
</template>
<script>
import SideBar from '../common/SideBar'

export default {
    components:{
        SideBar
    }
}
</script>
<style scoped>
.container{
    height: 600px;
}
.el-header, .el-footer {
    background-color: #B3C0D1;
    color: #333;
    text-align: center;
    line-height: 60px;
  }

  .el-aside {
    background-color: #D3DCE6;
    color: #333;
    text-align: center;
    line-height: 200px;
  }

  .el-main {
    background-color: #E9EEF3;
    color: #333;
    text-align: center;
    line-height: 160px;
  }

  body > .el-container {
    margin-bottom: 40px;
  }

  .el-container:nth-child(5) .el-aside,
  .el-container:nth-child(6) .el-aside {
    line-height: 260px;
  }

  .el-container:nth-child(7) .el-aside {
    line-height: 320px;
  }
</style>
