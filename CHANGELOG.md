# 更新日志

> MDUT-Extend 版本发布日志。原版 MDUT 更新日志请参考 [SafeGroceryStore/MDUT](https://github.com/SafeGroceryStore/MDUT)。

## 2026-08-21 - `v1.4.0`

### 🌟 New Features / 新增
* 新增 Redis DoubleFree 漏洞利用支持
* 新增 Redis TDigest 漏洞利用支持

### 🐛 Bug Fixes / 修复
* 修复 Redis 计划任务无法彻底删除的问题 (Fixed [#26](https://github.com/DeEpinGh0st/MDUT-Extend-Release/issues/26))

## 2026-03-27 - `v1.3.1`

### 🛡 Security / 安全
* 解决 MongoDB 利用脚本源文件供应链投毒问题 (Fixed [#22](https://github.com/DeEpinGh0st/MDUT-Extend-Release/issues/22))

### 🐛 Bug Fixes / 修复
* 修复 MongoDB 存活探测异常问题 (Fixed [#21](https://github.com/DeEpinGh0st/MDUT-Extend-Release/issues/21))

## 2026-03-17 - `v1.3.0`

### 🌟 New Features / 新增
* 新增 MongoDB 类型数据库利用
* 新增数据库存活扫描功能 (Resolves [#7](https://github.com/DeEpinGh0st/MDUT-Extend-Release/issues/7))
* 新增 Redis CVE-2025-49844 和 CVE-2022-0543 利用
* 新增 Oracle 大文件模式上传和下载
* 新增 Mssql 的 Godpotato 等提权类型
* 新增 Mssql 加载 shellcode 功能
* 新增 Mssql 综合利用

### 🐛 Bug Fixes / 修复
* 修复 Oracle 的 ORA-12505 问题，现已支持 SID 和 service 连接方式 (Fixes [#9](https://github.com/DeEpinGh0st/MDUT-Extend-Release/issues/9))
* 修复某些情况下 Oracle 函数初始化失败问题
* 修复某些情况下 Oracle 执行 powershell 右括号缺失问题 (Fixes [#10](https://github.com/DeEpinGh0st/MDUT-Extend-Release/issues/10))
* 修复 Oracle 下载文件时 ORA-24345 问题 (Fixes [#10](https://github.com/DeEpinGh0st/MDUT-Extend-Release/issues/10))
* 修复 Redis 下 linux 计划任务名称随机化问题 (Fixes [#16](https://github.com/DeEpinGh0st/MDUT-Extend-Release/issues/16))
* 修复某些情况下 Postgresql 驱动程序异常问题 (Fixes [#18](https://github.com/DeEpinGh0st/MDUT-Extend-Release/issues/18))
* 修复某些场景下 Redis 主从复制失败问题 (Fixes [#19](https://github.com/DeEpinGh0st/MDUT-Extend-Release/issues/19))
* 修复某些场景下 Redis SocketException 问题 (Fixes [#20](https://github.com/DeEpinGh0st/MDUT-Extend-Release/issues/20))

### 🔨 Maintenance / 维护
* 升级 Jedis 依赖库至 4.2.3
* 移除不再支持的 HttpDao 文件和逻辑代码 (Closes [#2](https://github.com/DeEpinGh0st/MDUT-Extend-Release/issues/2))
* 优化分组 UI 和交互逻辑
* 移除代理功能设置

## 2024-12-19 - `v1.2.0`

### 🐛 修复
* 修复 redis 命令执行回显格式错乱和中文乱码问题
* 修复 mssql 下载文件只有 10kb 问题
* 修复 postgresql 命令执行问题，由 direct 改为 base64
* 修复 postgresql 读取中文目录和文件报错问题
* 修复 postgresql 文件删除失败问题

### ✨ 优化
* 优化 postgresql 文件管理显示以及兼容 linux
* 添加 postgresql 文件管理支持 pg func 和 cve 两种方式
* 添加 redis 主从同步前对数据进行磁盘同步
* 添加 postgresql 中 cve 方式读取文件
* 添加 Mssql 提权对 Godpotato 支持
* 其他代码优化

## 2024-08-29 - `v1.1.1`

> 紧急修复版本

### 🐛 修复
* 修复 postgresql 命令执行问题
* 修复链接关闭 null 问题

## 2024-08-20 - `v1.1.0`

### 🐛 修复
* 修复 mysql no select database 问题
* 修复 postgresql 命令执行 UTF-8 字符问题 (Fixes [#5](https://github.com/DeEpinGh0st/MDUT-Extend-Release/issues/5))
* 修复数据库链接遗留问题

### ✨ 优化
* 添加 socks5 代理支持
* 添加 redis windows 系统支持
* 添加 postgresql 文件管理功能
* 调整 redis 利用界面布局

## 2024-08-11 - `v1.0.0`

### 🐛 修复
* 修复 mysql 5.0 版本 udf 错误问题
* 修复 linux 下 redis ping 命令卡死问题
* 修复 mssql 的 CLR 激活问题
* 修复 redis 反弹 shell 后主进程结束问题
* 修复 oracle 连接时 ORA-28009 问题
* 修复 oracle 命令执行前缀问题
* 修复 oracle ShellUtil 编译错误问题

### ✨ 优化
* 添加分组管理功能
* 添加 mysql 驱动高低版本切换选项
* 添加 oracle 命令执行无前缀选项
* 添加 oracle 命令执行 noline 模式
* 优化 redis 无损写 SSH key
* 添加 redis 无损文件读写功能
* 去除原版启动提示
* 去除原版更新菜单
* 优化文字显示和交互体验