<template>
  <div>
    <div class="line"></div>
    <el-menu
      :default-active="activeIndex2"
      class="el-menu-demo"
      mode="horizontal"
      @select="handleSelect"
      background-color="#C1B3A3"
      text-color="white"
      active-text-color="#ffd04b"
      style="line-height: 80px">
      <el-menu-item >
        <img src="../assets/bihua.png" style="width: 60px;height: 60px">
        <span style="font-size: 15px; ">
          CPU_CHINA
        </span>
      </el-menu-item>
      <el-menu-item index="1">
        <span style="font-size: 20px; margin-left: 50px">
          Home
        </span>
      </el-menu-item>
      <el-submenu index="2">
        <template slot="title">
        <span style="font-size: 20px; ">
          Project
        </span>
        </template>
        <el-menu-item index="2-1">选项1</el-menu-item>
        <el-menu-item index="2-2">选项2</el-menu-item>
        <el-menu-item index="2-3">选项3</el-menu-item>
      </el-submenu>
      <el-submenu index="3">
        <template slot="title">
        <span style="font-size: 20px; ">
          Human Practices
        </span>
        </template>
        <el-menu-item index="2-1">选项1</el-menu-item>
        <el-menu-item index="2-2">选项2</el-menu-item>
        <el-menu-item index="2-3">选项3</el-menu-item>
      </el-submenu>
      <el-submenu index="4">
        <template slot="title">
        <span style="font-size: 20px; ">
          Model
        </span>
        </template>
        <el-menu-item index="2-1">选项1</el-menu-item>
        <el-menu-item index="2-2">选项2</el-menu-item>
        <el-menu-item index="2-3">选项3</el-menu-item>
      </el-submenu>

      <el-submenu index="5">
        <template slot="title">
        <span style="font-size: 20px; ">
          Notebook
        </span>
        </template>
        <el-menu-item index="2-1">选项1</el-menu-item>
        <el-menu-item index="2-2">选项2</el-menu-item>
        <el-menu-item index="2-3">选项3</el-menu-item>
      </el-submenu>
      <el-submenu index="6">
        <template slot="title">
        <span style="font-size: 20px; ">
          Team
        </span>
        </template>
        <el-menu-item index="2-1">选项1</el-menu-item>
        <el-menu-item index="2-2">选项2</el-menu-item>
        <el-menu-item index="2-3">选项3</el-menu-item>
      </el-submenu>
      <el-submenu index="7">
        <template slot="title">
        <span style="font-size: 20px; ">
          Contacts
        </span>
        </template>
        <el-menu-item index="2-1">选项1</el-menu-item>
        <el-menu-item index="2-2">选项2</el-menu-item>
        <el-menu-item index="2-3">选项3</el-menu-item>
      </el-submenu>
      <el-menu-item index="8">
        <span style="font-size: 20px; ">
          JudgingFrom
        </span>
      </el-menu-item>
    </el-menu>
  </div>
</template>

<script>
export default {
  name: 'Nav',
  data () {
    return {
      activeIndex: '1',
      activeIndex2: '0'
    }
  },
  methods: {
    handleSelect (key, keyPath) {
      console.log(key, keyPath)
    }
  }
}
</script>

<style scoped>
</style>
