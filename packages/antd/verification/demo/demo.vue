<template>
  <div class="wrapper">
    <xy-verification
      v-model="code"
      telephone="13800000831"
      @sendCode="sendCode"
      :is-send-code.sync="isSendCode"
      @verifyCode="verifyCode"
    />
  </div>
</template>
<script>
import XyVerification from "../src/index.vue";

export default {
  components: { XyVerification },
  data() {
    return {
      isSendCode: false,
      code: '',
    }
  },
  methods: {
    // 发送验证码
    sendCode() {
      setTimeout(() => {
        this.isSendCode = true;
      }, 1000)
    },
    // 校验验证码
    verifyCode(code) {
      // 校验成功后，你可能需要把状态重置
      this.isSendCode = false;
      // 如果需要在特定的时候清空验证码表单，那么需要手动设置
      this.code = '';
    }
  }
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