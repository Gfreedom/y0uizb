<template>
  <el-row>
    <el-col :span=24>
      <el-menu 
        :default-active="activeIndex2" 
        class="muen" 
        router 
        mode="horizontal"
        @select="handleSelect"
        background-color="#545c64"
        text-color="#fff"
        active-text-color="#ffd04b">
        <el-menu-item index="1">首页</el-menu-item>
        <el-submenu index="2">
          <template slot="title">共享</template>
          <el-menu-item index="2-1">海洋仪器设备</el-menu-item>
          <el-menu-item index="2-2">海洋行业标准</el-menu-item>
          <el-menu-item index="2-3">海洋期刊文献</el-menu-item>
          <el-menu-item index="2-4">海洋科研成果</el-menu-item>
         
        </el-submenu>
        <!-- <el-menu-item index="3"><a href="https://www.ele.me" target="_blank">Case</a></el-menu-item> -->
        <el-submenu index="3">
          <template slot="title">交易</template>
          <el-menu-item index="3-1">海洋渔业数据</el-menu-item>
          <el-menu-item index="3-2">海洋船舶数据</el-menu-item>
          <el-menu-item index="3-3">海洋油气数据</el-menu-item>
          <el-menu-item index="3-4">海洋旅游数据</el-menu-item>
        </el-submenu>
        <el-menu-item index="4"><a href=" " target="_blank">处理</a></el-menu-item>
         <el-submenu index="5">
          <template slot="title">挑战</template>
          <el-menu-item index="5-1">大数据挖掘</el-menu-item>
          <el-menu-item index="5-2">三维空间数据</el-menu-item>
          <el-menu-item index="5-3">大数据可视化</el-menu-item>
        </el-submenu>
        <el-menu-item index="6"><a href=" " target="_blank">关于我们</a></el-menu-item>
      </el-menu>
    </el-col>
    <!-- 右边用户信息以及登陆注册 -->
   <!--  <el-button-group>
      <el-button type="danger" size="small" round >login</el-button>
      <el-button type="success" size="small" round >regin</el-button>
    </el-button-group> -->
  </el-row>
</template>

<script>
export default{
  
}
</script>

<style scoped>
  
</style>