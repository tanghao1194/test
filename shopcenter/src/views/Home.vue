<template>
  <div class="home">
    <el-button type='primary'>测试按钮</el-button>
    <el-row>
        <el-col :span = 8> <el-button type = 'primary'>按钮左</el-button></el-col>
        <el-col :span = 16><el-button type = 'success' @click="tonewpage">按钮右</el-button></el-col>
    </el-row>
  </div>
</template>

<script>
// @ is an alias to /src


export default {
  name: 'Home',
  components: {
    
  },
  methods:{
   tonewpage(){
       this.$router.push('./new');
   }
  }
}
</script>
