<template>
  <div class="wrapper">
    <xy-wrapper>我是 wrapper 组件</xy-wrapper>
  </div>
</template>
<script>
import XyWrapper from "../src/index.vue";

export default {
  components: { XyWrapper },
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