<template>
  <div class="wrapper">
    <xy-frame url="http://so.cn" />
  </div>
</template>
<script>
import XyFrame from '../src/index.vue';

export default {
  components: {XyFrame},
}
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