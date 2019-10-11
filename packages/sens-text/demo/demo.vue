<template>
  <div class="wrapper">
    <antd-xy-sens-text text="13800000831" type="mobile"></antd-xy-sens-text>
    <antd-xy-sens-text text="xiyun_dev@xiyun.com.cn" type="email"></antd-xy-sens-text>
  </div>
</template>
<script>
import XySelectCity from "../src/index.vue";

export default {
  components: { XySensText },
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