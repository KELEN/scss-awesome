cssMixins封装了一些常用的样式，帮助你快速编写样式

- [定位](#position)
    - [绝对居中](#absolute-center)
    
- 形状
    - 三角形
    - 带边框三角形

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

## 形状
> shape.scss
### 三角形
| 参数 | 值 |
| --- | --- | 
| 方向  | top/right/bottom/left |
| 大小 | px |
| 颜色 | color值 |

```scss
@include triangle(top, 20px, #333);
```

### 带边框的三角形

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