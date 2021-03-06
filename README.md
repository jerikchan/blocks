# 禧云业务组件仓库

各业务组件目录结构说明：
- antd 目录中存放基于 AntDesignVue 开发的业务组件
- element 目录中存放基于 ElementUI 开发的业务组件
- vant 目录中存放基于 VantUI 开发的业务组件

#### 贡献组件
首先 fork 本仓库，然后在业务组件目录中执行以下命令：
```bash
$ xy block-create <your-component-name>
```
就会在当前目录中生成一个名为：your-component-name 的目录，目录结构如下：
```
your-component-name/
  demo/
    demo.vue
  src/
    index.vue
  package.json
  README.md
```
组件源码放在 src 目录中

请注意，为了能让你的组件能够正确在线上平台展示，所以务必准确在`package.json`中填写完整以下信息：
```json
"blockConfig": {
    // 组件标题
    "title": "内容组件",
    // 组件分类
    "categories": [
      "信息展示"
    ],
    // 截图，请在你的组件目录下附带组件截图的图片，在pr时，我们会上传并修改此项地址
    "screenshot": ""
  },
```

开发时为方便查看实时效果，你可以在 demo 目录中执行以下命令：
```bash
$ xy block-dev demo.vue
```
这时会开启一个默认带有 ant-design-ui 资源的预览开发服务，更多关于 block-dev 的用法请查看[禧云 CLI 文档](https://xiyun-international.github.io/xy/cli/plugins/block-dev.html)或[README](https://github.com/xiyun-international/xy/tree/master/packages/antd/xy-plugin-block-dev)