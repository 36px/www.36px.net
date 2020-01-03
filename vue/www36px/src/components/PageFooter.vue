
<style scoped>
.hello {
  background: #ccc;
  padding: 20px;
  line-height: 180%;
  color: #777;
  font-size: 15px;
}
</style>

<template>
  <div class="hello">
    <div>(C) 2020 36px.net</div>
    <div>三十六像素App加工厂 aka. 36px软件开发工作室</div>
    <div>地址：桂林市七星区信息产业园</div>
  </div>
</template>

<script>
export default {
  name: "PageFooter",
  props: {
    msg: String
  }
};
</script>
