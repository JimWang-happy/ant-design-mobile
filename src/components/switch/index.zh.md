# Switch 开关

开关选择器。

## 何时使用

- 需要表示开关状态/两种状态之间的切换时。
- 和 checkbox 的区别是，切换 switch 会直接触发状态改变，而 checkbox 一般用于状态标记，需要和提交操作配合。

<code src="./demos/demo1.tsx"></code>

<code src="./demos/demo2.tsx"></code>

### 属性

| 参数           | 说明             | 类型                              | 默认值  |
| -------------- | ---------------- | --------------------------------- | ------- |
| checked        | 指定当前是否打开 | `boolean`                         | `false` |
| defaultChecked | 初始是否打开     | `boolean`                         | `false` |
| loading        | 加载状态         | `boolean`                         | `false` |
| disabled       | 禁用状态         | `boolean`                         | `false` |
| beforeChange   | 变化前执行       | `(val: boolean) => Promise<void>` | -       |
| onChange       | 变化时回调函数   | `(val: boolean) => void`          | -       |
| checkedText    | 选中时的内容     | `ReactNode`                       | -       |
| uncheckedText  | 非选中时的内容   | `ReactNode`                       | -       |

### CSS 变量

| 属性            | 说明     | 默认值                     |
| --------------- | -------- | -------------------------- |
| --checked-color | 填充颜色 | `var(--adm-color-primary)` |
| --width         | 宽度     | `51px`                     |
| --height        | 高度     | `31px`                     |
| --border-width  | 边框宽度 | `2px`                      |
