<template>
  <template>
    <el-container>
      <el-header><!-- 头部区 -->
        Header
        <el-button type="info" @click="logout">退出</el-button>
      </el-header>
      <!-- 页面主体区域 -->
      <el-container>
        <!-- 侧边栏 -->
        <el-aside width="200px">Aside</el-aside>
        <!-- 右侧内容主体 -->
        <el-main>Main</el-main>
      </el-container>
    </el-container>
  </template>

  <script>
    export default {
      methods:{
        logout(){
          window.sessionStorage.clear();
          this.$router.push('/login');
        }
      }
    };
  </script>

  <style lang="less" scoped>

  </style>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
