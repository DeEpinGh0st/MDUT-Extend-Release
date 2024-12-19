<p align="center">
<img src="https://socialify.git.ci/DeEpinGh0st/MDUT-Extend-Release/image?description=1&language=1&name=1&owner=1&pattern=Floating%20Cogs&theme=Light" alt="WindowsBaselineAssistant"/>
<img src="https://img.shields.io/github/stars/DeEpinGh0st/MDUT-Extend-Release?style=flat" alt="GitHub Repo stars"/>
<img src="https://img.shields.io/github/downloads/DeEpinGh0st/MDUT-Extend-Release/total?style=flat" alt="GitHub Downloads (all assets, all releases)"/>
<img alt="GitHub Release" src="https://img.shields.io/github/release/DeEpinGh0st/MDUT-Extend-Release"/>
<img src="https://img.shields.io/github/release-date/DeEpinGh0st/MDUT-Extend-Release?style=flat" alt="GitHub Release Date"/>
<p>


##  更新日志

####  2024-12-19

发布v1.2.0

**修复**

> 修复redis命令执行回显格式错乱和中文乱码问题
>
> 修复mssql下载文件只有10kb问题
>
> 修复postgresql命令执行问题,由direct改为base64
>
> 修复postgresql读取中文目录和文件报错问题
>
> 修复postgresql文件删除失败问题

**优化**

> 优化postgresql文件管理显示以及兼容linux
>
> 添加postgresql文件管理支持pg func和cve两种方式
>
> 添加redis主从同步前对数据进行磁盘同步
>
> 添加postgresql中cve方式读取文件
>
> 添加Mssql提权对Godpotato支持
>
> 其他代码优化

**SHA1**

> MDUT-Extend-1.2.0.zip  ADEA3261855D4C7F0D9002E4A8416EBE0D6E4397  
> redis-module-extend-windows.zip 3CF830E474D5E2C22DB2198DD5A52AC36DBBAD30  
> redis-module-extend-linux.zip  750B6EBA467B636C7A1A2C80B80AD32414D1BC40  

####  2024-08-20

发布v1.1.0

> 启动时需添加 **-Doracle.jdbc.javaNetNio=false** JVM选项  

**修复**

>修复mysql no select databse问题  
>修复postgresql命令执行UTF-8字符问题 #5  
>修复数据库链接遗留问题  

**优化**

>添加socks5代理支持  
>添加redis windows系统支持  
>添加postgresql文件管理功能  
>调整redis利用界面布局   

**SHA1**

> MDUT-Extend-1.1.0.zip  993062938583FEEA8A8E6FA9272A1DEB1CC08095  
> redis-module-extend-windows.zip 1477798592D5F7711E2D04FFCC10BD8F13336E23  
> redis-module-extend-linux.zip  750B6EBA467B636C7A1A2C80B80AD32414D1BC40  

####  2024-08-11

发布v1.0.0

**修复**

>修复mysql5.0版本udf错误问题  
>修复linux下redis ping命令卡死问题  
>修复mssql的CLR激活问题  
>修复redis反弹shell后主进程结束问题  
>修复oracle连接时ORA-28009问题  
>修复oracle命令执行前缀问题  
>修复oracle ShellUtil编译错误问题  

**优化**

>添加分组管理功能  
>添加mysql驱动高低版本切换选项  
>添加oracle命令执行无前缀选项  
>添加oracle命令执行noline模式  
>优化redis无损写SSH key  
>添加redis无损文件读写功能  
>去除原版启动提示  
>去除原版更新菜单  
>优化文字显示和交互体验  

**SHA1**

> MDUT-Extend-1.0.0.zip 209EB58C3463DB32477EE6F88D92EC0E1A88BA0F  
> redis-module-extend.zip 750B6EBA467B636C7A1A2C80B80AD32414D1BC40  

