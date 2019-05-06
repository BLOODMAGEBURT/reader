<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>Essential Links</h2>
    <el-radio-group v-model="radio">
      <el-radio :label="3">备选项1</el-radio>
      <el-radio :label="6">备选项2</el-radio>
      <el-radio :label="9">备选项3</el-radio>
      <el-radio :label="10">备选项4</el-radio>
    </el-radio-group>
    <p>被选中的{{ radio }}</p>

  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      radio: 6
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  h1, h2 {
    font-weight: normal;
  }

  ul {
    list-style-type: none;
    padding: 0;
  }

  a {
    color: #42b983;
  }
  .el-radio {
    display: block;
    margin-bottom: 20px;
  }
  .el-radio:last-child {
    margin-right: 30px;
  }
</style>
