# 常用样式

> 对应的scss文件 `normal.scss`

主要功能是提供一些浏览器前缀自动补全写法

## 禁止用户选中文本

```scss
@include disableSelect;
// or
@extend %disableSelect;
```

## 清楚浮动

```scss
@include clearfix;
// or
@extend %clearfix;
```

## 文本溢出省略号

```scss
@include textEllipsis;
// or
@extend %textEllipsis;
```