# code-langua#  开发环境一键安装脚本

一个 PowerShell 脚本，用于在 Windows 系统上一键安装完整的开发环境。

##  功能特性

-  **一键安装**：自动安装 Python、Node.js、Java、C++ Build Tools
-  **智能检测**：自动检测是否已安装组件
-  **环境配置**：自动配置 JAVA_HOME 和 PATH 环境变量
-  **权限管理**：自动请求管理员权限
-  **进度显示**：实时显示安装进度和结果

##  安装组件

| 组件 | 版本 | 说明 |
|------|------|------|
| Python | 3.13 | 最新的 Python 版本 |
| Node.js | 22 LTS | 长期支持版本 |
| OpenJDK | 22 | Microsoft 发行的 OpenJDK |
| Visual Studio Build Tools | 2022 | C++ 开发工具链 |

##  快速开始

### 方法一：一键安装（推荐）

以**管理员身份**打开 PowerShell，然后运行：

```powershell
# 使用原始链接直接运行
irm https://raw.githubusercontent.com/你的用户名/仓库名/main/install.ps1 | iex
ge
