# 定位

> 对应的scss文件 `position.scss`

# 绝对居中

> 兼容ie7

```scss
@include absoluteCenter($w, $h);
```
##### 参数

| 参数 | 单位 | 必须 |
| --- | --- |  --- |
| 宽 | px | 是 |
| 高 | px | 是 |

#####  用法
```scss
@include absoluteCenter(300px, 500px);
```