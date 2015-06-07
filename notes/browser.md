[link](http://compass-style.org/reference/compass/support/)

```
@import "compass/support";

@debug browsers();

// or
compass interactive
>> browser-versions(chrome)

$supported-browsers: chrome firefox;
$browsers-minimum-versions: ("ie": "8");
```

```
.webdemo-sec {
    position: relative;
    width: 100px;
    top: 10px;
    @include box-shadow(1px 1px 3px 2px #cfcecf);
}
/* line 18, ../sass/screen.scss */
.webdemo-sec {
  position: relative;
  width: 100px;
  top: 10px;
  -moz-box-shadow: 1px 1px 3px 2px #cfcecf;
  -webkit-box-shadow: 1px 1px 3px 2px #cfcecf;
  box-shadow: 1px 1px 3px 2px #cfcecf;
}

```
