# drawer组件
基于 element-ui drawer抽屉组件封装，具体使用方法与 element-ui 分页组件一致

## 基础使用
``` html
<template>
  <pk-drawer
  :visible.sync="drawer"
  ></pk-drawer>
</template>
```

```javascript
<script>
export default {
  data () {
    return {
      drawer: false
    }
  },
}
</script>
```
