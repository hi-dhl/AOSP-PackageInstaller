## AOSP-PackageInstaller

### 前言

注意：Android 10 及更高版本中, 相比于Android 9 及更低版本，PackageInstaller源码位置有所变动

### PackageInstaller源码所在位置

安装器PackageInstaller是系统内置的应用程序，用于安装和卸载应用<br/>

在 Android 9 及更低版本中，软件包安装和权限控制功能包含在 PackageInstaller 软件包 (//packages/apps/PackageInstaller) 中。在 Android 10 及更高版本中，权限控制功能位于单独的软件包 PermissionController (//packages/apps/PermissionController)，这两个软件包在 Android 10 中的位置如下图所示，更多信息点击这里前往[Android 权限](https://source.android.google.cn/devices/tech/config?hl=zh-cn)（需要科学上网）<br/>

![](http://cdn.51git.cn/2020-02-25-15825131880109.jpg)

<br/>

**Android 9 及更低版本中 ：**

软件包安装和权限控制功能源码路径：packages/apps/PackageInstaller

**Android 10 及更高版本：**

* 权限控制功能PermissionController源码路径：packages/apps/PermissionController/
* 安装器PackageInstaller源码路径：frameworks/base/packages/PackageInstaller/

### 在线查看源码方式

* [AOSP-PackageInstaller](https://github.com/hi-dhl/AOSP-PackageInstaller/tree/android-10.0.0_r14): 包含了安装器PackageInstaller(7.1.2、8.1.0、9.0.0、10.0.0)的源码，可以切换分之查看，跟随 Android 版本更新，你永远可以看到最新的源代码
* [aospxref](http://aospxref.com/)：这是一个在线查看Android源码网站，服务器在阿里云访问速度很快
* [googlesource-PackageInstaller](https://android.googlesource.com/platform/frameworks/base/+/refs/tags/android-10.0.0_r14/packages/PackageInstaller/)：这是安装器PackageInstaller在googlesource上的地址，需要科学上网

### AOSP-PackageInstaller使用方式

AOSP-PackageInstaller 包含了安装器PackageInstaller(7.1.2、8.1.0、9.0.0、10.0.0)的源码，可以切换分之查看<br/>
![source](http://cdn.51git.cn/2020-02-29-source.png)

**默认master分支上没有任何代码，clone的时候需要切换到对应版本分支上进行查看**

```
git clone git@github.com:hi-dhl/AOSP-PackageInstaller.git PackageInstaller  -b android-10.0.0_r14
```

### 总结

AOSP-PackageInstaller 跟随 Android 版本更新，你永远可以看到最新的源代码，如果你同我一样喜欢研究Android源码，可以关注我 GitHub 上的 AOSP-PackageInstaller

