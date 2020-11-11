---
id: position
title: Position
sidebar_label: Position
---

## position

设置 position 布局方式和位置偏移量

使用示例

```jsx
import {position} from '@redchili/retouch';

const style = css({
  ...position({type: 'relative'}),
});
```

生成的 CSS

```css
div {
  position: relative;
}
```

参数

| 参数   |           类型           | 默认值 | 是否可选 |
| ------ | :----------------------: | -----: | -------: |
| type   | "relative" 、 "absolute" | "none" |     必选 |
| top    |          String          |      / |     可选 |
| right  |          String          |      / |     可选 |
| bottom |          String          |      / |     可选 |
| left   |          String          |      / |     可选 |
