<template>
  <div class="wrapper">
    <xy-timeline leftWidth="100px">
      <span slot="left">2018-10-10 10:00</span>
      <span slot="right">我是右侧内容</span>
    </xy-timeline>
    <xy-timeline leftWidth="100px" status="success">
      <span slot="left">2018-10-10 10:00</span>
      <span slot="right">我是右侧内容</span>
    </xy-timeline>
    <xy-timeline leftWidth="100px" status="wait" :isShowLine="false">
      <span slot="left">2018-10-11 10:00</span>
      <div slot="right">
        <p>我是很多内容</p>
        <p>我是很多内容</p>
        <p>我是很多内容</p>
        <p>我是很多内容</p>
        <p>我是很多内容</p>
      </div>
    </xy-timeline>
  </div>
</template>
<script>
import XyTimeLine from "../src/index.vue";

export default {
  components: { XyTimeLine }
};
</script>
<style scoped>
.wrapper {
  width: 600px;
  height: 300px;
  border: 1px dashed silver;
  margin: 0 auto;
  padding: 10px;
}
</style>