# README

# ue4/fastbuild

### fastbuild  v0.99

### ue4\.22.3

* \\Engine\\Source\\Programs\\UnrealBuildTool\\Configuration\\BuildConfiguration.cs
* \\Engine\\Source\\Programs\\UnrealBuildTool\\Configuration\\UEBuildPlatform.cs
* \\Engine\\Source\\Programs\\UnrealBuildTool\\Platform\\Windows\\UEBuildWindows.cs
* \\Engine\\Source\\Programs\\UnrealBuildTool\\Platform\\Windows\\VCEnvironment.cs
* \\Engine\\Source\\Programs\\UnrealBuildTool\\System\\ActionGraph.cs
* \\Engine\\Source\\Programs\\UnrealBuildTool\\System\\FASTBuild.cs
* \\Engine\\Source\\Programs\\UnrealBuildTool\\Configuration\\ModuleRules.cs

### 添加环境变量/Add Environment variable

Add FastBuild Path：

C:\\FastBuild\\FASTBuild\-Windows\-x64\-v0.99       

C:\\FastBuild\\FASTBuild\-Windows\-x64\-v0.99\\FBuild.exe

### 分布式编译/Distributed compilation

Add Environment variable

变量名/Variable name：FASTBUILD\_BROKERAGE\_PATH

变量值/Variable value：\\\\192.168.1.45\\FASTBuildBroker

PC\_B：添加环境变量/Add Environment variable，启动/and start fbuildworker.exe

PC\_A：使用/use vs2017

##\# 

## `BuildConfiguration.cs`

`public bool bAllowFastbuild = true;//开关/switch`



[https://github.com/yass007/FASTBuildMonitor](https://github.com/yass007/FASTBuildMonitor)




