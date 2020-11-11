---
id: size
title: Size
sidebar_label: Size
---

## size

设置块级元素的宽高，支持 css 的简写值方式

使用示例

```jsx
import {size} from '@redchili/retouch';

const style = css({
  ...size('12px'),
});
```

生成的 CSS

```css
div {
  width: 12px;
  height: 12px;
}
```

参数

| 参数 |  类型  | 默认值 | 是否可选 |
| ---- | :----: | -----: | -------: |
| size | String |     \  |     必选 |


