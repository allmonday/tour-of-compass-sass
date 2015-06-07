```
.analyzer-logo {
    //background-image: inline-image("analyzer.png")
    background-image: image-url("analyzer.png");  // add cache bruster
    /* config.rb 中可以指定文件路径, 以及是否使用相对地址 */
}
```

```
compass compile -e production --force // 覆盖重写已有文件

config.rb
environment = :production
```
