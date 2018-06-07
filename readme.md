cssMixins封装了一些常用的样式，帮助你快速编写样式

- [常规](#normal)
    - [文本溢出](#text-ellipsis)

- [定位](#position)
    - [绝对居中](#absolute-center)
    - [绝对定位水平居中](#absolute-horizontal-center)
    
- [形状](#shape)
    - [三角形](#triangle)
    - [带边框三角形](#border-triangle)
    
## normal
常规样式

### text ellipsis
文本溢出省略号

```scss
@include textEllipsis;
```


## position
> position.scss

### absolute center
绝对居中定位

| 参数 | 值 |
| --- | --- | 
| 宽 | px |
| 高 | px |

```scss
@include absoluteCenter(200px, 300px);
```

绝对定位水平居中
```scss
@include absoluteHorizontalCenter;
// or
@extend %absoluteHorizontalCenter;
```

## shape
> shape.scss
### triangle
三角形

| 参数 | 值 |
| --- | --- | 
| 方向  | top/right/bottom/left |
| 大小 | px |
| 颜色 | color值 |

```scss
@include triangle(top, 20px, #333);
```

### border triangle 
带边框的三角形

| 参数 | 值 |
| --- | --- | 
| 方向  | top/right/bottom/left |
| 大小 | px |
| 颜色 | color值 |
| 边框粗细 | px |
| 边框颜色 | px | 

```scss
@include borderTriangle(top, 20px, #333, 2px, red);
```