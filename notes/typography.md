- links
- lists
- text
- vertical rhythm

link
```
@import "compass/typography/links";

a {
    @include hover-link();
    @include link-colors(#00c, #0cc, #c0c, #ccc, #cc0);
    @include unstyled-link();
}
```

list 
```
.list-unstyled {
    @include no-bullets();
}
.list-unstyled-li {
    @include no-bullet();
}
.list-inline {
    @include inline-list(); 
}

.list-horizontal {
    @include horizontal-list(10px, right); 
    // @include horizontal-list(false); 
}

.list-inline-block {
    @include inline-block-list();
}
```

text
```
.text-force-wrap {
    @include force-wrap();
}

.container {
    width: 100px;
}

.text-nowrap {
    @include nowrap();
}

.text-ellipsis {
    @include ellipsis();
}

for mozilla
>> compass install compass/ellipsis
$use-mozilla-ellipsis-binding: true;

output: 

.text-ellipsis {
  white-space: nowrap;
  overflow: hidden;
  -ms-text-overflow: ellipsis;
  -o-text-overflow: ellipsis;
  text-overflow: ellipsis;
  -moz-binding: url('/stylesheets/xml/ellipsis.xml#ellipsis');
}


.text-hide {
    // @include hide-text();
    @include squish-text();
}
.btn-find {
    // @include replace-text("http://cdn.qq.com/find-btn.png");
    @include replace-text-with-dimensions("local.png");
}
```

vertical rhythm
```
$base-font-size: 16px;
$base-line-height: 24px;
@include establish-baseline();
body {
    @include debug-vertical-alignment();
}

h1 {
    @include adjust-font-size-to(48px);
}

h2 {
    @include adjust-font-size-to(36px);
}

h3 {
    @include adjust-font-size-to(24px);
}

h4 {
    @include adjust-font-size-to(21px);
}

h5 {
    @include adjust-font-size-to(18px);
}

h6 {
    @include adjust-font-size-to(16px);
}

p {
    @include adjust-font-size-to(14px);
    @include leader();
    @include trailer();
}

```
