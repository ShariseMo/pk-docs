# 分页组件
基于 element-ui 分页组件封装，具体使用方法与 element-ui 分页组件一致

## 基础使用
`total` 数据总大小
``` html
<template>
  <pk-pagination :total="pagination.total" />
</template>
```

## 事件绑定
使用方法和 element-ui 分页组件一致
``` html
<template>
  <pk-pagination
    :total="pagination.total"
    @size-change="handleSizeChange"
    @current-change="handlePageChange"
  >
  </pk-pagination>
</template>
```

```javascript
<script>
export default {
  data () {
    return {
      current: 1
    }
  },
  methods: {
    handleSizeChange () {},
    handleNextChange () {}
  }
}
</script>
```