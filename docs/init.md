---
id: init
title: 初始化
sidebar_label: 初始化
slug: /
---

## 简介
Retouch 是包含了一系列返回 Style Object 的函数库。可在 React 直接使用，也可和 emotion、styled components 搭配使用。其作用主要有下面的几点：
1. 简化书写 css ，通过对 css 自定义的简写封装，如 size 函数，省略分别定义 width、height 等来简化代码
2. 复用大量常见样式，如单行省略号的样式封装到一个函数里
3. 整理在项目开发中积累大量 css 通用样式，布局，使用 npm 分享复用

以上几点作用在使用 sass 或 tailwind css 等 css 优化方案也都有相应解决，但 Retouch 只导出 Style Object，支持 css in js ，获得完整的编程语言支持，在灵活和多样性上更好。

## 安装

```bash
yarn add @redchili/retouch
```

## 使用
搭配 emotion 使用
``` jsx
/** @jsx jsx */
import {
  css,
  jsx
} from "@emotion/core";
import {
  bg,
  padding,
  font
} from "@redchili/retouch";

const color = "white";

const style = css({
  ...bg({ color: "hotpink" }), // NOTE: 设置背景颜色
  ...padding("32px"), // NOTE: 设置 padding
  ...font({ size: "24px" }) // NOTE: 设置字体
});

export default function Option() {
  return (
    <div
      css={css`
        ${style};
        border-radius: 4px;
        &:hover {
          color: ${color};
        }
      `}
    >
      Hover to change color.
    </div>
  );
}
```