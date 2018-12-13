# Android单元测试
>主流单元测试框架AndroidTest和Robolectric,两者的区别如下

* AndroidTest 是基于Android环境，运行在Android机器上
* Robolectric 是直接运行在JVM上，速度比AndroidTest要快，无需准备Android环境。
    - 注意：对于一些测试对象依赖度较高而需要解除依赖的场景，我们可以借助Mock框架。
# Robolectric环境配置
