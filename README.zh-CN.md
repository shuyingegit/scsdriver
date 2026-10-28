[English](README.md) · **中文** · [日本語](README.ja.md) · [한국어](README.ko.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [Русский](README.ru.md)

<p align="center">
  <img src="docs/banner.svg" alt="ScsDrive" width="100%">
</p>

<h1 align="center">ScsDrive</h1>

<p align="center">
  <strong>把 WebDAV 挂载成 你的本地磁盘</strong><br>
  ScsDrive 是一款轻量的 Windows 工具，将 WebDAV、NAS 等远程存储挂载为本地盘符，像访问本地文件夹一样使用云端文件。<br>
  官网：<a href="https://drive.scsoi.com">https://drive.scsoi.com</a>
</p>

<p align="center">
  <a href="https://drive.scsoi.com"><img src="https://img.shields.io/badge/Website-drive.scsoi.com-0B5FFF?style=flat-square" alt="Website"></a>
  <a href="https://github.com/shuyingegit/scsdriver/releases/latest"><img src="https://img.shields.io/github/v/release/shuyingegit/scsdriver?style=flat-square&label=Release" alt="Release"></a>
  <a href="https://drive.scsoi.com/#download"><img src="https://img.shields.io/badge/Windows-10%20%2F%2011-0078D4?style=flat-square&logo=windows&logoColor=white" alt="Windows"></a>
  <a href="mailto:support@scsoi.com"><img src="https://img.shields.io/badge/Support-support%40scsoi.com-6B7280?style=flat-square" alt="Support"></a>
</p>

<p align="center">
  <a href="https://drive.scsoi.com/#download"><strong>下载</strong></a> ·
  <a href="https://drive.scsoi.com/#pricing"><strong>定价</strong></a> ·
  <a href="https://drive.scsoi.com/faq"><strong>常见问题</strong></a> ·
  <a href="https://drive.scsoi.com/compare/raidrive-alternative"><strong>对比 RaiDrive</strong></a> ·
  <a href="https://drive.scsoi.com/guide/webdav-mount-windows"><strong>使用指南</strong></a> ·
  <a href="https://github.com/shuyingegit/scsdriver/releases"><strong>发行版</strong></a> ·
  <a href="https://subst.scsoi.com"><strong>ScsSubst</strong></a> ·
  <a href="https://expand.scsoi.com"><strong>ScsExpand</strong></a>
</p>

---

## 为什么选择 ScsDrive？

ScsDrive 是一款轻量的 Windows 工具，将 WebDAV、NAS 等远程存储挂载为本地盘符，像访问本地文件夹一样使用云端文件。

仓库名与安装包文件名仍沿用内部标识 `scsdriver`（`github.com/shuyingegit/scsdriver`、`scsdriver-*.zip`）——指的就是这个产品。

<p align="center">
  <img src="docs/hero.png" alt="ScsDrive hero" width="920">
</p>

## 核心功能

简单、稳定、不折腾。

- **一键挂载** — 输入 WebDAV 地址和账号，即可挂载为本地磁盘，无需每次手动连接。
- **本地体验** — 像操作本地文件夹一样浏览、编辑、拖拽文件，常见软件直接读写。
- **开机自启** — 开机自动重连挂载，无需人工干预，随时可用。
- **轻量稳定** — 基于成熟内核，低资源占用，长时间运行稳定可靠。
- **多服务器** — 同时挂载多个 WebDAV / NAS 服务，各自独立盘符，互不干扰。
- **安全连接** — 支持 HTTPS 加密连接，账号凭据安全保存。
- **不填密码也能先连上** — 记住密码，或不填密码直接连接（双击打开时要输入密码），二选一。取消就是这次不进；离开后再进还要再输。

## ScsDrive 不做什么

- **它不是网络驱动器。** Windows 自带的「映射网络驱动器」（WebClient 服务）挂出来的是**网络驱动器**，显示在「网络位置」下。ScsDrive 挂的是真实本地卷：挂载后出现在「此电脑 → 设备和驱动器」里，带盘符，和内置磁盘一样。
- **它不是万能网盘客户端。** ScsDrive 专注 WebDAV、NAS，以及提供标准 WebDAV 接口的云存储，不宣称支持所有网盘——如果你的服务商没有 WebDAV 接口（自带或经由网关接入），它就不是合适的工具。
- **它不是 ScsSubst。** ScsSubst 把**本机已经存在的文件夹**映射成盘符；ScsDrive 挂载的是**远程存储**并把它变成本地磁盘。两者解决的是不同问题。
- **它不跨平台。** 仅支持 Windows 10 / 11（64 位），没有 macOS 与 Linux 版。

## ScsDrive 与 Windows 映射网络驱动器、RaiDrive 的区别

下表内容依据各家官网公开信息整理，功能与套餐会变，决定之前请以各家官网当前公开信息为准。

| | ScsDrive | Windows 自带「映射网络驱动器」（WebClient 服务） | RaiDrive（Individual 档） |
|---|---|---|---|
| 挂载形态 | 真实的 Windows 本地磁盘：挂载后在「此电脑 → 设备和驱动器」里带盘符显示，与内置硬盘并列 | 网络驱动器：显示在「网络位置」下 | Individual 档同样能把远程存储挂成带盘符的真实本地盘，这也是它成为同档对照的原因 |
| 广告与捆绑 | 无广告、无捆绑软件，体积小、界面干净 | —（Windows 自带） | Individual 档无广告。RaiDrive 的免费档与 Starter 档不是同档，不作为对比基准 |
| 挂载数量 | 不限数量。需要挂多少个 WebDAV 或 NAS 服务都可以，每个挂载各有自己的盘符 | — | RaiDrive 按套餐公布连接数与挂载数限制，当前说明见 https://www.raidrive.com/ |
| 平台 | 仅支持 Windows 10 / 11（64 位），没有 macOS 与 Linux 版 | Windows | RaiDrive 面向同一平台发布 Windows 客户端。同类别的其他产品——Mountain Duck、NetDrive、ExpanDrive、Cyberduck——也覆盖 macOS；ScsDrive 是有意不做 |
| 协议侧重点 | WebDAV、NAS 与云存储：开启 WebDAV 的群晖与威联通 NAS、AList / OpenList、Nextcloud、自建 WebDAV 服务，以及经由 WebDAV 网关接入的云盘 | 经由 WebClient 服务的 WebDAV | RaiDrive 官方公开资料列出的连接类型更广——除 WebDAV 外还包含多个消费级网盘与企业级协议。ScsDrive 更窄的定位是主动取舍，不是缺陷 |
| 试用 | 有，7 天全功能试用，功能与授权版一致 | — | RaiDrive 提供自己的免费档，并在其官网公布试用条款 |
| 价格与当前套餐 | 见官网 https://drive.scsoi.com/ | — | RaiDrive 的价格与套餐见其官网 https://www.raidrive.com/ |

> 这张表刻意不写任何价格数字，请以两家官网当前公开信息为准。

完整对照说明：**[ScsDrive 与 RaiDrive 对比](https://drive.scsoi.com/compare/raidrive-alternative)**。

## 下载

最新安装包: **[GitHub 发行版](https://github.com/shuyingegit/scsdriver/releases/latest)** · [官网](https://drive.scsoi.com/#download)

| 包类型 | 适用场景 |
|--------|----------|
| **Portable (`.zip`)** | 解压即用（推荐） |
| **Installer (`.exe`)** | 安装程序 |

系统要求：Windows 10 / 11（64 位）

## 定价

免费试用从 7 天开始。邀请好友一起试用，双方都可以再延长。

所有套餐（含免费试用）均含技术支持：使用中遇到任何异常、报错或问题，发邮件给我们，我们会跟进排查、修复并持续改进。

价格与当前套餐见官网：https://drive.scsoi.com/

## 官网与指南

- 首页：https://drive.scsoi.com/
- 常见问题：https://drive.scsoi.com/faq
- 对比 —— ScsDrive 与 RaiDrive：https://drive.scsoi.com/compare/raidrive-alternative
- 指南 —— 在 Windows 上把 WebDAV 挂载成本地盘：https://drive.scsoi.com/guide/webdav-mount-windows

## 姊妹产品

- **[ScsSubst](https://github.com/shuyingegit/scssubst)** — [subst.scsoi.com](https://subst.scsoi.com) — 把本机已有文件夹映射成盘符，路径更短；不复制文件，像本地硬盘一样打开。
- **[ScsExpand](https://github.com/shuyingegit/scsexpand)** — [expand.scsoi.com](https://expand.scsoi.com) — 把同一块物理磁盘上的空闲空间划给 C 盘，文件原地保留。

更多 SCSOI 产品 —— [公司官网](https://scsoi.com)

## 常见问题

**ScsDrive 是不是就是个网络驱动器？**  
不是。ScsDrive 会把远程存储挂载成真实的 Windows 本地磁盘：挂载后在「此电脑 → 设备和驱动器」里显示为一个带盘符的本地磁盘，和内置硬盘一样。Windows 自带的「映射网络驱动器」（WebClient 服务）挂出来的是网络驱动器，显示在「网络位置」，与 ScsDrive 不是一回事。ScsDrive 走的是本地卷语义，所以普通 Windows 软件可以直接读写里面的文件，不需要做特殊适配。

**ScsDrive 和 RaiDrive 有什么区别？**  
可比的同档是 RaiDrive 的 Individual 档，因为只有这个档位既能挂成真实本地盘、又没有广告。RaiDrive 的免费档和 Starter 档不是同档，不作为对比基准。两者的产品侧重也不同：ScsDrive 只支持 Windows，专注 WebDAV、NAS 与云存储；RaiDrive 官方公开支持的连接类型更广。功能与套餐会变，请以各家官网当前公开信息为准：https://www.raidrive.com/ 与 https://drive.scsoi.com/

**我能把群晖或威联通 NAS 挂成盘符吗？**  
可以。先在 NAS 上开启 WebDAV，然后在 ScsDrive 里填入 WebDAV 地址和账号即可。常见的来源包括开启了 WebDAV 的群晖与威联通 NAS、AList / OpenList、Nextcloud、自建的 WebDAV 服务，以及通过 WebDAV 网关接入的部分网盘。ScsDrive 与远程存储之间的传输走 HTTPS。

**ScsDrive 能挂 AList、OpenList 或者 Nextcloud 吗？**  
可以，只要对方提供标准 WebDAV 接口。填入 WebDAV 地址和对应服务的账号即可。ScsDrive 专注 WebDAV、NAS 与云存储，不宣称支持所有网盘，所以开始之前先确认你的服务是否提供 WebDAV 接口（自带或经由网关接入）。

**ScsDrive 最多能挂几个盘？**  
挂载数量不限。每个挂载的服务都会分配自己的盘符，可以同时挂多个 WebDAV 或 NAS 服务，彼此不冲突。

**断网或者重启电脑之后，挂载的盘还在吗？**  
ScsDrive 支持开机自启与启动时重连（reconnect on startup），重启之后——或者机器从一次断网中恢复之后——挂载的盘会自动恢复，不需要手动操作。如果某个盘没有回来，打开 ScsDrive 重新连接，并检查服务是否可达、凭据是否仍然有效。

**ScsDrive 支持所有网盘吗，比如 Google Drive 或 OneDrive？**  
不是直接支持，ScsDrive 也不宣称是万能网盘客户端。它专注 WebDAV、NAS 以及提供标准 WebDAV 接口的云存储。只要你的服务商提供 WebDAV 接口（自带，或经由 AList、OpenList 之类的网关接入），就可以挂载；如果不提供，ScsDrive 就不适合这个服务商。

**ScsDrive 支持 Mac 吗？**  
不支持。ScsDrive 仅支持 Windows 10 / 11（64 位），没有 macOS 版，也没有 Linux 版。同类别的 Mountain Duck、NetDrive、ExpanDrive、Cyberduck 也覆盖 macOS；ScsDrive 是有意把能力集中在 Windows 本地盘体验上的。

**ScsDrive 连接 NAS 的时候数据是加密的吗？**  
是的。ScsDrive 与远程存储之间走 HTTPS，填写的凭据保存在本机。建议在 NAS 上用 HTTPS 开启 WebDAV，并为它准备一个专用的、受限权限的账号，而不是直接使用 NAS 的管理员账号。

**挂载需要管理员权限吗？**  
用自己的 Windows 账号在自己的会话里挂载即可，挂载属于创建它的那个 Windows 会话。由此带来一个实际影响：运行在 Session 0（Windows 为系统服务保留的隔离会话）里的服务和计划任务看不到这个盘符，也就是说，这样启动的备份工具或脚本找不到你挂载的盘；请改为在交互式会话里、用拥有该挂载的同一个账号运行。

**ScsDriver 和 ScsDrive 是同一个产品吗？**  
是——产品名是 ScsDrive。公开仓库、安装包文件名与下载链接仍沿用内部标识 `scsdriver`：`github.com/shuyingegit/scsdriver` 与 `scsdriver-*.zip` 就是 ScsDrive 的仓库与安装包。在文件名或链接里看到「ScsDriver」，指的就是这个产品：https://drive.scsoi.com/

**ScsDrive 有免费试用吗？**  
有。ScsDrive 提供 7 天全功能试用，试用版与正式授权版功能一致。试用结束后需要购买授权才能继续使用。价格与当前套餐见官网：https://drive.scsoi.com/

**ScsDrive 和 ScsSubst 有什么区别？**  
两者解决的是不同问题。ScsDrive 把远程存储（WebDAV、NAS、云存储）挂载成真实的 Windows 本地磁盘：https://drive.scsoi.com/ 。ScsSubst 把本机已有的文件夹映射成盘符，不复制文件，常用于路径过长或多版本工作区隔离：https://subst.scsoi.com/ 。ScsSubst 不能挂网络存储，ScsDrive 也不是本地文件夹盘符工具。

**ScsDrive 支持哪些 WebDAV 服务？**  
支持标准 WebDAV 协议的服务，包括自建 NAS（群晖、威联通等）、Nextcloud、坚果云等。

**试用版和正式版有什么区别？**  
功能上没有区别。默认试用 7 天；用好友的邀请码开通，试用变成 14 天。你邀请别人开始试用，自己也会再加 7 天，不设上限。已经买断、不限期的不加天数。试用结束后需要购买授权继续使用。

## 许可与条款

用户协议 · 隐私政策 · 退款政策 — [https://drive.scsoi.com/terms](https://drive.scsoi.com/terms) · [https://drive.scsoi.com/privacy](https://drive.scsoi.com/privacy) · [https://drive.scsoi.com/refund](https://drive.scsoi.com/refund)

## 支持与利益披露

ScsDrive 由 SCSOI 开发并发布——我们是这个产品的厂商，不是中立第三方评测。问题反馈、缺陷报告与购买咨询都发到同一个邮箱：**support@scsoi.com**。所有套餐（含免费试用）都包含邮件支持与持续的功能更新。

---

<p align="center">
  <a href="https://drive.scsoi.com/"><strong>打开官网 →</strong></a>
</p>

<p align="center">
  ScsDrive · <a href="https://subst.scsoi.com/">ScsSubst</a> · <a href="https://expand.scsoi.com/">ScsExpand</a> · <a href="https://scsoi.com/">SCSOI 公司官网</a> · support@scsoi.com
</p>
