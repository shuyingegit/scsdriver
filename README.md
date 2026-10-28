**English** · [中文](README.zh-CN.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · [Русский](README.ru.md)

<p align="center">
  <img src="docs/banner.svg" alt="ScsDrive" width="100%">
</p>

<h1 align="center">ScsDrive</h1>

<p align="center">
  <strong>Mount WebDAV as a Local Drive</strong><br>
  ScsDrive is a lightweight Windows tool that mounts WebDAV, NAS and remote storage as local drive letters — use your cloud files like a local folder.<br>
  Official site: <a href="https://drive.scsoi.com">https://drive.scsoi.com</a>
</p>

<p align="center">
  <a href="https://drive.scsoi.com"><img src="https://img.shields.io/badge/Website-drive.scsoi.com-0B5FFF?style=flat-square" alt="Website"></a>
  <a href="https://github.com/shuyingegit/scsdriver/releases/latest"><img src="https://img.shields.io/github/v/release/shuyingegit/scsdriver?style=flat-square&label=Release" alt="Release"></a>
  <a href="https://drive.scsoi.com/#download"><img src="https://img.shields.io/badge/Windows-10%20%2F%2011-0078D4?style=flat-square&logo=windows&logoColor=white" alt="Windows"></a>
  <a href="mailto:support@scsoi.com"><img src="https://img.shields.io/badge/Support-support%40scsoi.com-6B7280?style=flat-square" alt="Support"></a>
</p>

<p align="center">
  <a href="https://drive.scsoi.com/#download"><strong>Download</strong></a> ·
  <a href="https://drive.scsoi.com/#pricing"><strong>Pricing</strong></a> ·
  <a href="https://drive.scsoi.com/faq"><strong>FAQ</strong></a> ·
  <a href="https://drive.scsoi.com/compare/raidrive-alternative"><strong>vs RaiDrive</strong></a> ·
  <a href="https://drive.scsoi.com/guide/webdav-mount-windows"><strong>Guide</strong></a> ·
  <a href="https://github.com/shuyingegit/scsdriver/releases"><strong>Releases</strong></a> ·
  <a href="https://subst.scsoi.com"><strong>ScsSubst</strong></a> ·
  <a href="https://expand.scsoi.com"><strong>ScsExpand</strong></a>
</p>

---

## Why ScsDrive?

ScsDrive is a lightweight Windows tool that mounts WebDAV, NAS and remote storage as local drive letters — use your cloud files like a local folder.

The repository and the installer file names still use the internal id `scsdriver` (`github.com/shuyingegit/scsdriver`, `scsdriver-*.zip` installers) — that is this product.

<p align="center">
  <img src="docs/hero.png" alt="ScsDrive hero" width="920">
</p>

## Key Features

Simple, stable, hassle-free.

- **One-click Mount** — Enter your WebDAV URL and credentials to mount as a local drive. No manual reconnection needed.
- **Native Experience** — Browse, edit and drag files like a local folder. Apps can read/write directly.
- **Auto-start** — Automatically reconnects on boot. Always available, no manual intervention.
- **Lightweight & Stable** — Built on a mature kernel. Low resource usage, reliable for long-running use.
- **Multi-server** — Mount multiple WebDAV / NAS services at once. Independent drive letters, no conflicts.
- **Secure Connection** — HTTPS encrypted connection. Credentials stored securely.
- **Connect before you type a password** — Choose remember password, or connect without one (password when you open the drive). Cancel means leave this time; open again later and it asks again.

## What ScsDrive Is NOT

- **Not a network drive.** Windows' own "Map network drive" (the WebClient service) creates a *network drive* that lives under "Network locations". ScsDrive mounts a real local volume instead: the drive appears under "This PC → Devices and drives" with a drive letter, exactly like an internal disk.
- **Not a universal cloud-drive client.** ScsDrive focuses on WebDAV, NAS and cloud storage that expose a standard WebDAV endpoint. It does not claim to support every cloud provider — if your provider has no WebDAV endpoint (directly or through a gateway), ScsDrive is not the right tool for it.
- **Not ScsSubst.** ScsSubst maps a folder that **already exists on your PC** to a drive letter. ScsDrive mounts **remote** storage as a local disk. Different products, different jobs.
- **Not cross-platform.** Windows 10 / 11 (64-bit) only — there is no macOS or Linux build.

## ScsDrive vs. Windows mapped network drives and RaiDrive

Everything below is based on the public information each vendor publishes. Features and plans change, so confirm the current state on each vendor's own site before you decide.

| | ScsDrive | Windows "Map network drive" (WebClient service) | RaiDrive — Individual tier |
|---|---|---|---|
| Mount form | A real Windows local disk: it appears under "This PC → Devices and drives" with a drive letter, next to your internal disks | A network drive: it appears under "Network locations" | The Individual tier can also mount remote storage as a real local drive with a drive letter, which is why it is the comparable tier |
| Ads and bundled software | No ads and no bundled software. Small footprint, clean interface | — (part of Windows) | The Individual tier carries no ads. RaiDrive's free tier and Starter tier are a different tier and are not the basis of this comparison |
| Number of mounts | No limit — mount as many WebDAV or NAS services as you need, each with its own drive letter | — | RaiDrive publishes the connection and mount limits that come with its plans; see https://www.raidrive.com/ |
| Platform | Windows 10 / 11 (64-bit) only. There is no macOS or Linux build | Windows | RaiDrive publishes a Windows client for the same platform. Other products in this category — Mountain Duck, NetDrive, ExpanDrive, Cyberduck — also cover macOS; ScsDrive deliberately does not |
| Protocol focus | WebDAV, NAS and cloud storage: Synology and QNAP with WebDAV enabled, AList / OpenList, Nextcloud, self-hosted WebDAV services, and cloud drives exposed through a WebDAV gateway | WebDAV through the WebClient service | RaiDrive's public materials list a wider range of connection types — several consumer cloud drives plus enterprise protocols in addition to WebDAV. ScsDrive's narrower focus is a deliberate scope choice, not a defect |
| Trial | Yes — a 7-day full-featured trial, with the same features as the licensed version | — | RaiDrive offers its own free tier and publishes its trial terms on its own site |
| Price and current plans | Listed on the official site: https://drive.scsoi.com/ | — | RaiDrive lists its own prices and plans on https://www.raidrive.com/ |

> This table deliberately carries no price figures — check the current information on each official site.

Full side-by-side walkthrough: **[ScsDrive vs RaiDrive](https://drive.scsoi.com/compare/raidrive-alternative)**.

## Download

Latest builds: **[GitHub Releases](https://github.com/shuyingegit/scsdriver/releases/latest)** · [Website](https://drive.scsoi.com/#download)

| Package | Use when |
|--------|----------|
| **Portable (`.zip`)** | Unzip and run — recommended |
| **Installer (`.exe`)** | Classic setup |

Requirements: Windows 10 / 11 (64-bit)

## Pricing

The free trial starts at 7 days. Invite a friend to try it, and both of you can extend it.

All plans (including the free trial) include technical support: if you hit any error or issue, email us — we will investigate, fix it, and keep improving.

Pricing and current plans are listed on the official site: https://drive.scsoi.com/

## Official site and guides

- Home: https://drive.scsoi.com/
- FAQ: https://drive.scsoi.com/faq
- Comparison — ScsDrive vs RaiDrive: https://drive.scsoi.com/compare/raidrive-alternative
- Guide — how to mount WebDAV as a local drive on Windows: https://drive.scsoi.com/guide/webdav-mount-windows

## Sister products

- **[ScsSubst](https://github.com/shuyingegit/scssubst)** — [subst.scsoi.com](https://subst.scsoi.com) — map existing local folders to drive letters — shorter paths, no file copying.
- **[ScsExpand](https://github.com/shuyingegit/scsexpand)** — [expand.scsoi.com](https://expand.scsoi.com) — grow C: using free space from the same physical disk — files stay in place.

More from SCSOI — [SCSOI company site](https://scsoi.com)

## FAQ

**Is ScsDrive just another network drive?**  
No. ScsDrive mounts the remote storage as a real Windows local disk: after mounting, the drive appears under "This PC → Devices and drives" with a drive letter, exactly like an internal disk. Windows' own "Map network drive" feature (the WebClient service) is different — it creates a network drive that appears under "Network locations". ScsDrive deliberately uses local-volume semantics, so ordinary Windows software can read and write the files without special handling.

**How is ScsDrive different from RaiDrive?**  
The comparable tier is RaiDrive's Individual tier, because that is the tier that can mount remote storage as a real local drive and carries no ads. RaiDrive's free tier and Starter tier are not the same tier, so they are not the basis of this comparison. The two products then differ in scope: ScsDrive is Windows-only and focused on WebDAV, NAS and cloud storage, while RaiDrive publicly supports a wider range of connection types. Features and plans change — check each vendor's current public information: https://www.raidrive.com/ and https://drive.scsoi.com/

**Can I mount my Synology or QNAP NAS as a drive letter?**  
Yes. Enable WebDAV on the NAS, then add the WebDAV address and your account in ScsDrive. Common sources are Synology and QNAP with WebDAV turned on, AList / OpenList, Nextcloud, self-hosted WebDAV services, and some cloud drives exposed through a WebDAV gateway. The connection to the remote storage runs over HTTPS.

**Can I mount AList, OpenList or Nextcloud with ScsDrive?**  
Yes — as long as the service exposes a standard WebDAV endpoint. Enter the WebDAV URL and the account you use for that service. ScsDrive is focused on WebDAV, NAS and cloud storage; it is not a universal client for every cloud provider, so check that your provider offers a WebDAV endpoint (directly or through a gateway) before you start.

**How many drives can I mount at the same time?**  
There is no limit on the number of mounts. Each mounted service gets its own drive letter, so you can mount several WebDAV or NAS services at the same time and they do not conflict with each other.

**What happens to my mounted drive after a reboot or a dropped network?**  
ScsDrive can start with Windows and reconnect on startup, so after a reboot — or after the machine came back from a network outage — the mounted drive is restored without manual work. If a drive does not come back, open ScsDrive and reconnect, and check that the service is reachable and that the credentials are still valid.

**Does ScsDrive support every cloud drive, such as Google Drive or OneDrive?**  
Not directly, and ScsDrive does not claim to be a universal cloud client. ScsDrive focuses on WebDAV, NAS and cloud storage that expose a standard WebDAV endpoint. If your provider offers a WebDAV endpoint — directly or through a gateway such as AList or OpenList — you can mount it. If it does not, ScsDrive is not the right tool for that provider.

**Does ScsDrive work on Mac or Linux?**  
No. ScsDrive supports Windows 10 / 11 (64-bit) only, and there is no macOS or Linux build. Other products in this category — Mountain Duck, NetDrive, ExpanDrive and Cyberduck — also cover macOS; ScsDrive deliberately concentrates on the Windows local-disk experience.

**Is the connection to my NAS encrypted?**  
Yes. ScsDrive talks to the remote storage over HTTPS, and the credentials you enter are stored on the computer. Use a dedicated account with limited rights on the NAS instead of its administrator account.

**Do I need administrator rights to mount a drive?**  
Mount the drive from your own Windows account, in your own session. A mount belongs to the Windows session that created it, and that has one practical consequence: services and scheduled tasks running in Session 0, the isolated system session Windows keeps for system services, do not see the drive letter, so a backup tool or script started that way will not find your mounted drive. Run such a task in an interactive session as the same user who owns the mount.

**Is ScsDriver the same product as ScsDrive?**  
Yes — ScsDrive is the product name. The public repository, the installer file names and the download links still use the internal identifier `scsdriver`: `github.com/shuyingegit/scsdriver` and the `scsdriver-*.zip` installers are the ScsDrive repository and installers. If you ran into "ScsDriver" in a file name or a link, it is this product: https://drive.scsoi.com/

**Is there a free trial for ScsDrive?**  
Yes. ScsDrive has a 7-day full-featured trial, and the trial has the same features as the licensed version. After the trial a license is needed to keep using it. Pricing and current plans are listed on the official site: https://drive.scsoi.com/

**What is the difference between ScsDrive and ScsSubst?**  
They solve different problems. ScsDrive mounts remote storage — WebDAV, NAS, cloud storage — as a real Windows local disk: https://drive.scsoi.com/ . ScsSubst maps an existing local folder to a drive letter without copying files, and is used for long paths or for keeping several workspaces apart: https://subst.scsoi.com/ . ScsSubst cannot mount network storage, and ScsDrive is not a local-folder drive-letter tool.

**Which WebDAV services does ScsDrive support?**  
Supports any standard WebDAV service, including self-hosted NAS (Synology, QNAP, etc.), Nextcloud, Nutstore and more.

**What is the difference between trial and licensed versions?**  
Same features. The trial is 7 days; start it with a friend’s invite code and it becomes 14. When someone starts a trial with your code, you also gain 7 days, with no cap. Lifetime licenses don’t add days. After the trial, buy a license to keep using it.

## License & terms

Terms · Privacy · Refunds — [https://drive.scsoi.com/terms](https://drive.scsoi.com/terms) · [https://drive.scsoi.com/privacy](https://drive.scsoi.com/privacy) · [https://drive.scsoi.com/refund](https://drive.scsoi.com/refund)

## Support and disclosure

ScsDrive is developed and published by SCSOI — we are the vendor of this product, not a neutral third-party reviewer. Questions, bug reports and purchase questions all reach the same inbox: **support@scsoi.com**. Every plan, including the free trial, includes email support and ongoing feature updates.

---

<p align="center">
  <a href="https://drive.scsoi.com/"><strong>Open website →</strong></a>
</p>

<p align="center">
  ScsDrive · <a href="https://subst.scsoi.com/">ScsSubst</a> · <a href="https://expand.scsoi.com/">ScsExpand</a> · <a href="https://scsoi.com/">SCSOI company site</a> · support@scsoi.com
</p>
