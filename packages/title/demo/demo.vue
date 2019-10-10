<template>
  <div class="wrapper">
    <xy-title large>大号标题</xy-title>
    <xy-title no-top-margin>小号标题</xy-title>
    <xy-title no-top-margin show-icon large sub-title="副标题">
      拥有右侧内容的大号标题
      <a-button slot="right" type="primary">右侧内容</a-button>
    </xy-title>
    <xy-title no-top-margin show-icon sub-title="副标题">
      拥有右侧内容的小号标题
      <span slot="right">右侧内容</span>
    </xy-title>
  </div>
</template>
<script>
import XyTitle from "../src/index.vue";
import { Button as AButton } from "ant-design-vue";
import "ant-design-vue/lib/button/style/css";

export default {
  components: { XyTitle, AButton }
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