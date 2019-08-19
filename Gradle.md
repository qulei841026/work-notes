#Gradle
+ 传递(transitive)
+ 排除(exclude)
+ 强制(force)
+ 动态版本(+)
```
    implementation('com.xxx:xxx:1.0.0@aar') {
        transitive = true
        changing = true
        force = true
        exclude group: 'com.xxx', module: 'xxx'
    }
```