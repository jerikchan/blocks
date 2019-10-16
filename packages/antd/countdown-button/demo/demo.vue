<template>
  <div class="wrapper">
    <xy-countdown-button @click="onClick" :is-send.sync="isSend"></xy-countdown-button>
  </div>
</template>
<script>
import XyContext from '../src/index.vue';

export default {
  components: {XyContext},
  data() {
    return {
      isSend: false,
    }
  },
  methods: {
    onClick() {
      // 模拟接口请求
      setTimeout(() => {
        this.isSend = true;
      }, 1000)
      // 真实接口请求
      // this.$post('api', {phone: input}).then(res => {
      //   if (res) {
      //     this.isSend = true;
      //   } else {
      //     this.$message({
      //       message: res.message,
      //       type: 'error',
      //     });
      //     this.isSend = false;
      //   }
      // }).catch(() => {
      //   this.isSend = false;
      // })
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