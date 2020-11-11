---
id: flex
title: Flex
sidebar_label: Flex
---

## flexSpaceBetween
使用 flex 布局，两端对齐的函数

使用示例

```jsx
import {flexSpaceBetween} from '@redchili/retouch';

const style = css({
  ...flexSpaceBetween(),
});
```

生成的 CSS

```css
div {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}
```

参数

| 参数      |       类型        | 默认值 | 是否可选 |
| --------- | :---------------: | -----: | -------: |
| direction | "row" 、 "column" |  "row" |     可选 |

## flexCenter
使用 flex 布局实现内部元素垂直水平居中

使用示例
```jsx
import {flexCenter} from '@redchili/retouch';

const style = css({
  ...flexCenter(),
});
```

生成的 CSS
```css
div {
    display: flex;
    justify-content: center;
    align-items: center;
}
```