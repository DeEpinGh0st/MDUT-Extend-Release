<p align="center">
<img src="https://socialify.git.ci/DeEpinGh0st/MDUT-Extend-Release/image?description=1&language=1&name=1&owner=1&pattern=Floating%20Cogs&theme=Light" alt="WindowsBaselineAssistant"/>
<img src="https://img.shields.io/github/stars/DeEpinGh0st/MDUT-Extend-Release?style=flat" alt="GitHub Repo stars"/>
<img src="https://img.shields.io/github/downloads/DeEpinGh0st/MDUT-Extend-Release/total?style=flat" alt="GitHub Downloads (all assets, all releases)"/>
<img alt="GitHub Release" src="https://img.shields.io/github/release/DeEpinGh0st/MDUT-Extend-Release"/>
<img src="https://img.shields.io/github/release-date/DeEpinGh0st/MDUT-Extend-Release?style=flat" alt="GitHub Release Date"/>
<p>


##  更新日志

####  2026-03-27

发布v1.3.1

🛡**Security**

- 解决MongoDB利用脚本源文件供应链投毒问题(Fixed [#22](https://github.com/DeEpinGh0st/MDUT-Extend-Release/issues/22))

🐛 Bug Fixes

- 修复MongoDB存活探测异常问题(Fixed [#21](https://github.com/DeEpinGh0st/MDUT-Extend-Release/issues/21))



####  2026-03-17

发布v1.3.0

🌟 New Features
- 新增MongoDB类型数据库利用
- 新增数据库存活扫描功能(Resolves #7)
- 新增Redis CVE-2025-49844和CVE-2022-0543利用
- 新增Oracle大文件模式上传和下载
- 新增Mssql的Godpotato等提权类型
- 新增Mssql加载shellcode功能
- 新增Mssql综合利用

🐛 Bug Fixes
- 修复Oracle的ORA-12505问题，现已支持SID和service连接方式(Fixes #9)
- 修复某些情况下Oracle函数初始化失败问题
- 修复某些情况下Oracle执行powershell右括号缺失问题(Fixes #10)
- 修复Oracle下载文件时ORA-24345问题(Fixes #10)
- 修复Redis下linux计划任务名称随机化问题(Fixes #16)
- 修复某些情况下Postgresql驱动程序异常问题(Fixes #18)
- 修复某些场景下Redis主从复制失败问题(Fixes #19)
- 修复某些场景下Redis SocketException问题(Fixes #20)


🔨 Maintenance
- 升级Jedis依赖库至最4.2.3
- 移除不再支持的HttpDao文件和逻辑代码(Closes #2)
- 优化分组UI和交互逻辑
- 移除代理功能设置
