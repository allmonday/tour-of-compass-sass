normalize:

- `gem install compass-normalize`


modules:
- base: html, body, 文字大小, 边距
- html5: article, nav, ... 
- links: a
- typography: b, strong, sub, sup
- embeds: img, svg
- groups: code, pre..
- forms: button, input, textarea
- tables: td, th

```
@import "normalize-version";  /* 导入子模块声明 */
/*! 1*/
@import "normalize/base";
/*! 2*/
@import "normalize/html5";
/*! 3*/
@import "normalize/links";
```

```
/* 只重置某个class下的 */
@import "compass/reset/utilities";

.reset-sec {
    @include nested-reset;
}
```
