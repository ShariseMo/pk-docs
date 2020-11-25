# 筛选器

可展开/收起的头部筛选器

### 收起
<img src="/pk-filter/images/collapse.jpg" />

### 展开
<img src="/pk-filter/images/expand.jpg" />

``` html
<!-- 单用时可以补充class="app-bg" 或其他一些样式 -->
<pk-filter 
  @toggleShow="showFilter = !showFilter"         
  @onFilter="handleFilter"
  @onReset="handleReset"
  :show="showFilter" 
  style="background: #fafafa" 
  class="app-bg">
  <div class="g-filter-content" slot="filter-content">
    <!-- 筛选条件1 -->
    <div class="m-filter-item" >
      <p class="label">活动类型</p>
      <p class="form-item">
        <el-input/>
      </p>
    </div>
    <!-- 筛选条件2 -->
    <div class="m-filter-item" >
      <p class="label">活动类型</p>
      <p class="form-item">
        <el-input/>
      </p>
    </div>
    <!-- 其他筛选条件 -->
  </div>
</pk-filter>
```

``` javascript
import pkFilter from '@/components/pk-filter/index';
export default{
  components: { pkFilter },
  data(){
    return {
      showFilter: false
    }
  },
  methods: {
    handleFilter(){},
    handleReset(){}
  }
}
```


## Attributes
 
|  参数   | 说明             |  类型    | 可选值 | 默认值 |
|  :----  | :----          | :----     | :----  | :----  |
| show   | 控制筛选器展开/收起 | Boolean | true/false | false |


## Events
|  事件名称    | 说明       |  回调参数   |
|  :----  | :----          | :----     | 
| toggleShow   | 当筛选器展开/收起时触发事件 |  | 
| onFilter   | 点击筛选时触发事件 |  | 
| onReset   | 点击重置时触发事件 |  | 