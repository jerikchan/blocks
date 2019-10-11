<template>
  <div class="wrapper">
    <a-button @click="visible = true">点击选择城市</a-button>
    <xy-select-city
      v-if="visible"
      :initCity="cityList"
      @submitSelected="submitSelectedCity"
      :url="`https://www.easy-mock.com/mock/5d521ffe2fa9ed158bb10abe/example/tree`"
    />
  </div>
</template>
<script>
import XySelectCity from "../src/index.vue";

export default {
  components: { XySelectCity },
  data() {
    return {
      cityList: ['130200'],
      visible: false,
    }
  },
  methods: {
    // 提交选中城市 code
    submitSelectedCity() {
      this.visible = false;
    },
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