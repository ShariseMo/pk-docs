# dialogue组件
基于 element-ui dialogue组件封装，具体使用方法与 element-ui dialogue组件一致

## 基础使用
`show` 是否显示 Dialog
`width` Dialog 的宽度
``` html
<template>
  <pk-dialogue
      title="测试"
      :show="show"
      width="50%"
    >
      <template v-slot:content>
        <div></div>
      </template>
      <template v-slot:footer>
        <el-button>取 消</el-button>
        <el-button type="info">确 定</el-button>
      </template>
    </pk-dialogue>
</template>
```

```javascript
<script>
export default {
  data () {
    return {
      show: false
    }
  },
}
</script>
```
