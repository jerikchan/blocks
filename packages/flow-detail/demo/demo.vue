<template>
  <div class="wrapper">
    <xy-flow-detail :data="data" />
  </div>
</template>
<script>
import XyFlowDetail from '../src/index.vue';

export default {
  components: {XyFlowDetail},
  data() {
    return {
      data: []
    }
  }
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