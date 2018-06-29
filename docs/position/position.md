# 定位

> 对应的scss文件 `position.scss`

## 绝对居中

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

## 雪碧图背景定位

```scss
@include absoluteCenter($w, $h);
```
##### 参数

| 参数 | 说明 | 值 |
| --- | --- |  --- |
| $list | class数组，按顺序编写 |
| $size | 每个雪碧图的大小 |
| $tb | 从上到下 | 默认: true |

#####  用法
```scss
$sp: icon-apple, icon-banana, icon-orange, icon-pig;
@include bgPosition($sp, 40, false);
```
```css
.icon-apple { background-position: 0 0; }
.icon-banana { background-position: -40px 0; }
.icon-orange { background-position: -80px 0; }
.icon-pig { background-position: -120px 0; }
```
