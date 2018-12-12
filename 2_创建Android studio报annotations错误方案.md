### 创建Android studio报annotations 冲突处理，异常信息如下
```
Error:Execution failed for task ':app:preDebugAndroidTestBuild'.
> Conflict with dependency 'com.android.support:support-annotations' in project ':app'. Resolved versions for app (26.1.0) and test app (27.1.1) differ. See https://d.android.com/r/tools/test-apk-dependency-conflicts.html for details.
```
### 解决办法如下方式：
* 在build.gradle添加方式一
```
android {
    ...
}
configurations.all {
    resolutionStrategy.force 'com.android.support:support-annotations:27.1.1'
}
dependencies {
    ...
}
```
* 在build.gradle添加方式二
```
android {
    ...
}
dependencies {
    androidTestCompile('com.android.support:support-annotations:27.1.1') {
        force = true
    }
}
```