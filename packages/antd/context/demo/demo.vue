<template>
  <div class="wrapper">
    <xy-context
      :breadcrumb="[
    { name: '服务商中心', path: ''},
    { name: '协作费管理', path: ''}, 
    { name: '账单详情' }
  ]"
      title="账单详情"
      tag="审核中"
      :tag-status="5"
    >
      <p>我是内容区</p>
      <p>我是内容区</p>
      <p>我是内容区</p>
      <p>我是内容区</p>
      <p>我是内容区</p>
      <p>我是内容区</p>
      <p>我是内容区</p>
      <p>我是内容区</p>
      <div slot="right">
        <a-button type="primary">打印账单</a-button>
      </div>
    </xy-context>
  </div>
</template>
<script>
import XyContext from '../src/index.vue';
// import lodash from 'lodash';


export default {
  components: {XyContext},
}
</script>
<style scoped>
.wrapper {
  width: 600px;
  /* height: 300px; */
  border: 1px dashed silver;
  margin: 0 auto;
  padding: 10px;
}
</style>