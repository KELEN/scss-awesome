# 常用样式

> 对应的scss文件 `animation.scss`

动画定义

!> 由于IE8以及更早版本不支持animation

## animation-delay线性生成

| 参数 | 说明 | 值 |
| --- | --- | -- |
| cls | 类名 | '.list-item' |
| num | 个数 |  20 |
| start | 开始延迟的毫秒数 | 200 |
| step | 每次递增的毫秒数 | 50 | 
| reverse | 是否反向递增 | 默认：false |

```scss
@include animationDelay('.list-item', 4, 200, 50);
```
结果
```css
.list-item:nth-child(1) { animation-delay: 200ms; }
.list-item:nth-child(2) { animation-delay: 250ms; }
.list-item:nth-child(3) { animation-delay: 300ms; }
.list-item:nth-child(4) { animation-delay: 350ms; }
```

## transition-delay线性生成

| 参数 | 说明 | 值 |
| --- | --- | -- |
| cls | 类名 | '.list-item' |
| num | 个数 |  20 |
| start | 开始延迟的毫秒数 | 200 |
| step | 每次递增的毫秒数 | 50 | 
| reverse | 是否反向递增 | 默认：false |

```scss
@include transitionDelay('.list-item', 4, 200, 50);
```
结果
```css
.list-item:nth-child(1) { transition-delay: 200ms; }
.list-item:nth-child(2) { transition-delay: 250ms; }
.list-item:nth-child(3) { transition-delay: 300ms; }
.list-item:nth-child(4) { transition-delay: 350ms; }
```