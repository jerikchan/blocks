<template>
  <div class="wrapper">
    <xy-countdown-button
      style="margin: 180px 240px"
     @click="onClick" :is-send.sync="isSend"></xy-countdown-button>
  </div>
</template>
<script>
import XyCountdownButton from '../src/index.vue';

export default {
  components: {XyCountdownButton},
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
  height: 400px;
  border: 1px dashed silver;
  margin: 50px auto;
  padding: 10px;
}
</style>