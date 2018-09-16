<template>
  <div class="pos">
    <!-- eleme组件库 -->
    <el-row>
      <el-col :span='7' class="pos-order" id="order-list">我是订单栏</el-col>
      <el-col>我是产品栏</el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  name: 'pos',
  mounted: function(){
    // 生命周期, 所有dom加载完成之后
    var orderHeight = document.body.clientHeight;
    document.getElementById("order-list").style.height = orderHeight + "px";
  }
}
</script>

<style scoped>
h1, h2 {
  font-weight: normal;
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
.pos-order{
  background-color: #F9FAFC;
  border-right: 1px solid #C0CCDA;
  height: 100%;
}
</style>
