# ue4/fastbuild

### fastbuild  v0.99

### ue4\.22.3中修改的文件

* \\Engine\\Source\\Programs\\UnrealBuildTool\\Configuration\\BuildConfiguration.cs
* \\Engine\\Source\\Programs\\UnrealBuildTool\\Configuration\\UEBuildPlatform.cs
* \\Engine\\Source\\Programs\\UnrealBuildTool\\Platform\\Windows\\UEBuildWindows.cs
* \\Engine\\Source\\Programs\\UnrealBuildTool\\Platform\\Windows\\VCEnvironment.cs
* \\Engine\\Source\\Programs\\UnrealBuildTool\\System\\ActionGraph.cs
* \\Engine\\Source\\Programs\\UnrealBuildTool\\System\\FASTBuild.cs
* \\Engine\\Source\\Programs\\UnrealBuildTool\\Configuration\\ModuleRules.cs

### 环境变量

Path 中添加 两个 FastBuild 的路径

C:\\FastBuild\\FASTBuild\-Windows\-x64\-v0.99       

C:\\FastBuild\\FASTBuild\-Windows\-x64\-v0.99\\FBuild.exe


### 分布式编译

添加环境：

变量名：FASTBUILD\_BROKERAGE\_PATH

变量值：\\\\192.168.1.45\\FASTBuildBroker //局域网中的共享文件夹地址



B机器中：添加环境变量，启动fastbuild中的fbuildworker.exe

A机器中：用vs编译

### 

## `BuildConfiguration.cs`

`public bool bAllowFastbuild = true;//这个就是启动fastbuild开关`

# 问题：

**每次点击生成，都会重新生成。所以，现在编译源码打开开关，编译游戏工程时候关闭。**


