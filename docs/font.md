---
id: font
title: Font
sidebar_label: Font
---

## font

设置文本的字体样式

使用示例

```jsx
import {font} from '@redchili/retouch';

const style = css({
  ...font({family: 'custom', size: '12px', color: 'red'}),
});
```

生成的 CSS

```css
div {
  font-family: custom;
  font-size: 12px;
  color: red;
}
```

参数

| 参数       |  类型  | 默认值 | 是否可选 |
| ---------- | :----: | -----: | -------: |
| family     | String |      / |     可选 |
| size       | String |      / |     可选 |
| color      | String |      / |     可选 |
| lineHeight | String |      / |     可选 |
| weight     | String |      / |     可选 |
