<template>
  <div>
	<!-- element-ui navMenu -->
	<el-menu theme="dark" :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect" :router=true>
	  <el-menu-item index="/">RestBoard</el-menu-item>
	  <el-menu-item index="/app">
	    App
	  </el-menu-item>
	  <el-menu-item index="/">Api</el-menu-item>
      <el-menu-item index="/">Request</el-menu-item>
      <el-menu-item index="/doc">Doc</el-menu-item>
	</el-menu>
	<!-- 占位符 -->
	<router-view></router-view>
	
  </div>
</template>

<script>
export default {
  data () {
    return {
      activeIndex: '/app'
    }
  },
  methods: {
    handleSelect (key, keyPath) {
      // console.log(key, keyPath)
    }
  }
}
</script>

<style scoped>

</style>
