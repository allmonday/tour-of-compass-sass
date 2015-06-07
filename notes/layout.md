- grid-background
- sticky-footer
- stretching

是个不太用到的模块

[link](http://compass-style.org/reference/compass/layout/)

```
.stretch-full {
    @include stretch(5px, 5px, 5px, 5px);
}
/* line 20, ../sass/screen.scss */
.stretch-full {
  position: absolute;
  top: 5px;
  bottom: 5px;
  left: 5px;
  right: 5px;
}
```

```
@include sticky-footer(30px);

<div id="root">
    <div id="root_footer">
    </div>
</div>
<div id="footer">
    footer content goes here
</div>
```
