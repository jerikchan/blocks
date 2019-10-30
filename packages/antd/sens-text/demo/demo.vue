<template>
  <div class="wrapper">
    <div style="margin: 150px 200px">
    <xy-sens-text text="13800000831" type="mobile"></xy-sens-text>
    <xy-sens-text text="xiyun_dev@xiyun.com.cn" type="email"></xy-sens-text>

    </div>
  </div>
</template>
<script>
import XySensText from "../src/index.vue";

export default {
  components: { XySensText },
};
</script>
<style scoped>
.wrapper {
  width: 600px;
  height: 400px;
  border: 1px dashed silver;
  margin: 50px auto;
  padding: 10px;
}
</style>