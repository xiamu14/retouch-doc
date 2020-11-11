---
id: init
title: 初始化
sidebar_label: 初始化
slug: /
---

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