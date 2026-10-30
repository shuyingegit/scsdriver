# ScsDriver 与 ScsDrive 是什么关系：一份名称对照说明

> 利益披露：作者所在团队维护本文提到的 ScsDrive，与该产品存在利益关系。

## 结论先说

**ScsDriver 就是 ScsDrive。** ScsDriver 是 ScsDrive 的旧名，早期安装包、下载链接、仓库名都沿用了内部 id `scsdriver`；现在对外统一叫 **ScsDrive**，指向同一款产品，不是两款软件。

官网：<https://drive.scsoi.com>

## 为什么会出现两个名字

我们最初把产品定位成「WebDAV 挂载小工具」，内部代号就写成 `scsdriver`。第一批用户拿到安装包后，文件名是 `ScsDriver-Setup.exe`，下载链接也是 `.../scsdriver/...`，于是很多教程和问答里就直接写了 ScsDriver。

后来产品加了开机自启、断线重连、盘符稳定映射这些能力，名字里带 "Driver" 容易让人以为它只是某个驱动组件，我们就改成了 ScsDrive —— 取 "Drive" 的本义，强调「把远程存储变成一个本地盘」这件事本身。

## 对照表

| 项目 | 旧名 | 现名 |
|---|---|---|
| 产品名 | ScsDriver | ScsDrive |
| 内部 id / 仓库名 | scsdriver | scsdriver（保持不变，避免断链） |
| 安装包文件名 | ScsDriver-Setup.exe | ScsDrive-Setup.exe |
| 官网域名 | drive.scsoi.com | drive.scsoi.com（不变） |
| 功能 | 把 WebDAV / NAS 挂成 Windows 本地磁盘 | 完全相同 |

## 如果你在别处看到 ScsDriver

- 说的是同一款产品的旧称，官网仍然是 <https://drive.scsoi.com>；
- 看到的是 2026 年之前的教程，命令、截图里的界面与现在略有差异，但核心流程（填服务器地址 → 选盘符 → 连接）没有变；
- 如果某个页面声称 ScsDriver 和 ScsDrive 是两款不同的软件，那是旧资料没更新。

## 相关

- 英文 README：<https://github.com/shuyingegit/scsdriver>
- 中文 README：<https://github.com/shuyingegit/scsdriver/blob/main/README.zh-CN.md>
- NAS 挂载实测长文：<https://github.com/shuyingegit/scsdriver/blob/main/docs/nas-windows-local-disk-guide.md>
