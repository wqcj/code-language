# code-langua#  开发环境一键安装脚本

一个 PowerShell 脚本，用于在 Windows 系统上一键安装完整的开发环境。

##  功能特性

-  **一键安装**：自动安装 Python、Node.js、Java、c++、git
-  **智能检测**：自动检测是否已安装组件
-  **环境配置**：自动配置 JAVA_HOME 和 PATH 环境变量
-  **权限要求**：需要管理员权限
-  **进度显示**：实时显示安装进度和结果

##  安装组件

| 组件 | 版本 | 说明 |
|------|------|------|
| Python | 3.13 | 最新的 Python 版本 |
| Node.js | 22 LTS | 长期支持版本 |
| OpenJDK | 22 | Microsoft 发行的 OpenJDK |
| git |25|
##  快速开始

##一键安装（推荐）

以**管理员身份**打开 PowerShell，然后运行：
```powershell
irm asheroto.com/winget | iex  #安装完成后可能会自动退出，需要再管理员运行一次
winget install --id Microsoft.PowerShell --source winget --silent #安装支持的powershell新版7.0版本
#注意下面的命令要在新安装的powershell7.0上运行，搜索栏搜一下
$url = "https://raw.githubusercontent.com/wqcj/code-language/refs/heads/colan/colan"
$outFile = "$env:USERPROFILE\Desktop\colan.ps1"
$content = (Invoke-WebRequest -Uri $url -UseBasicParsing).Content
$content | Out-File -FilePath $outFile -Encoding utf8NoBOM
cd "$env:USERPROFILE\Desktop"
.\colan.ps1

