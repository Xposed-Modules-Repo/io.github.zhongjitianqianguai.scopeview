<p align="center">
  <img src="assets/scopeview-logo.png" width="168" height="168" alt="域见 ScopeView icon">
</p>

<h1 align="center">域见 ScopeView</h1>

<p align="center">
  更新 LSP 模块要逐个下载，逛仓库找新模块也得反复点开，还看不清哪些模块同时作用于某个应用？我来帮你。
  <br>
  Updating LSP modules one by one, opening repo entries to find new modules, and unsure which modules target the same app? I'm here to help.
  <br>
  一眼看清哪些 LSPosed 模块作用于某个应用，不用再逐个点开查找。
  <br>
  See at a glance which LSPosed modules target an app, without opening them one by one.
  <br>
  集中查看模块更新，支持单个更新和批量更新。
  <br>
  Check module updates in one place and update them individually or in a batch.
  <br>
  域见是独立的 Root 配套工具，无需激活 LSPosed 模块也可使用原有功能。
  <br>
  ScopeView is a standalone Root companion utility; its existing features work without activating the LSPosed module.
</p>

<p align="center">
  <a href="https://github.com/Xposed-Modules-Repo/io.github.zhongjitianqianguai.scopeview/stargazers"><img src="https://img.shields.io/github/stars/Xposed-Modules-Repo/io.github.zhongjitianqianguai.scopeview?style=for-the-badge&amp;logo=github&amp;label=Star" alt="GitHub Stars"></a>
  <a href="https://t.me/ScopeView_Offical"><img src="https://img.shields.io/badge/Telegram-Official_Group-26A5E4?style=for-the-badge&amp;logo=telegram&amp;logoColor=white" alt="Telegram Official Group"></a>
  <a href="https://t.me/zhongjitianqianguai3"><img src="https://img.shields.io/badge/Telegram-Release_Channel-26A5E4?style=for-the-badge&amp;logo=telegram&amp;logoColor=white" alt="Telegram Release Channel"></a>
</p>

<p align="center">
  你的 Star ⭐ 是我持续更新的最大动力。
  <br>
  Your Star ⭐ is my biggest motivation to keep updating ScopeView.
</p>

<p align="center">
  <a href="https://github.com/Xposed-Modules-Repo/io.github.zhongjitianqianguai.scopeview/releases">公开下载 / Downloads</a> · <a href="https://github.com/Xposed-Modules-Repo/io.github.zhongjitianqianguai.scopeview">官方索引 / Official index</a>
</p>

## 主要功能 / Features

- **发现模块**：浏览最近更新和新收录模块，卡片直接查看简介与更新摘要；支持搜索、通道选择、隐藏已安装/已收藏、Star 排序、收藏和已读标记。<br>
  **Discover modules:** Browse recent updates and new listings with descriptions and release previews on each card; search, choose a channel, hide installed or saved modules, sort by stars, bookmark and track what you have read.
- **按需查看详情**：原地展开或打开详情，查看 README、发布说明和历史版本；APK 链接交给浏览器下载，已安装模块可进入现有更新流程。<br>
  **Details on demand:** Expand a card or open its details for the README, release notes and history. APK links open in your browser, while installed modules can use the existing update flow.
- **按应用查看模块**：查看一个应用被哪些模块选入作用域，显示应用名称、包名、图标及 Android 用户信息。<br>
  **Modules by app:** See which modules include an app in their scopes, with app names, package names, icons and Android user information.
- **查看模块更新**：跟随管理器选择的官方来源和通道，检查已安装模块详情并核对缓存；失败时保留已有结果，识别仅名称变化的更新。<br>
  **Check module updates:** Follow the Manager’s official source and channel, check installed-module details and reconcile cached results; retain existing results on failure and recognize version-name-only updates.
- **通知快捷入口**：默认开启，点击通知打开域见；授权 Root 和通知权限后，划掉后台仍保留入口，设置中可关闭并保存选择。<br>
  **Notification shortcut:** Enabled by default; tap to open ScopeView. With Root and notification permission granted, it remains after removing the app from Recents; turn it off in Settings with your choice saved.
- **优先显示更新**：有更新的模块始终排在前面，各组内保留你选择的排序规则。<br>
  **Updates first:** Modules with available updates always appear first, with your chosen sort order preserved within each group.
- **单个、多选或全部更新**：支持更新单个模块、勾选后“更新所选”或“更新全部”；Beta、Nightly 和多 APK 项目由你逐项选择或跳过，没有 APK 的更新需你确认跳过。<br>
  **Individual, selected or all updates:** Update one module, select several with Update selected or use Update all; choose or skip each Beta, Nightly, or multi-APK item, and explicitly skip updates with no APK.
- **并行下载、有序安装**：单独点击多个模块时，最多三个下载并行，安装仍逐个执行；同一模块不重复排队，域见自身最后更新。<br>
  **Parallel downloads, ordered installs:** Start up to three individual downloads in parallel while installation stays sequential; avoid duplicate requests for the same module and update ScopeView itself last.
- **取消剩余任务**：等待当前更新完成，再停止后续更新。<br>
  **Cancel remaining updates:** Let the current update finish, then stop the remaining items.
- **搜索与排序**：按名称或包名搜索，为应用、模块和作用域详情分别保存排序规则。<br>
  **Search and sort:** Search by name or package name and save separate sort preferences for apps, modules and scope details.
- **多语言界面**：默认跟随系统语言，也可手动选择简体中文、英文或俄语。<br>
  **Multiple languages:** Follow the system language by default or choose Simplified Chinese, English or Russian manually.
- **跳转管理器**：从模块详情打开 LSPosed 管理器中的对应模块。<br>
  **Open in Manager:** Open the corresponding module in LSPosed Manager from its details.

- **模块日志与诊断**：展开或收起模块发布说明，支持 Markdown；导出日志包含各模块的关联和状态快照，慢操作标明界面、模块与阶段。<br>
  **Module notes and diagnostics:** Expand or collapse Markdown release notes. Export logs with per-module associations and state snapshots, plus screen, module and stage context for slow operations.
- **安装包清理**：默认后台自动清理已安装或旧版本的缓存包与无任务使用的下载残余，扳手中可独立关闭或手动清理；保留待安装、较新版本、失败重试和自身更新核对所需文件。<br>
  **APK cleanup:** Automatically clear installed or older cached APKs and inactive download remnants by default; disable this separately or clean manually in Settings. Pending installs, newer versions, retry files and self-update verification files are retained.
- **忽略更新与卸载**：在模块卡片的“更多”中永久忽略该模块更新，扳手设置可恢复；忽略项保留显示和主动单独更新，不参与更新计数、批量更新或后台提醒。卸载交由系统确认，返回后扫描实际安装状态。<br>
  **Ignore updates and uninstall:** Permanently ignore a module through its card's More menu and restore it in Settings. Ignored modules remain visible and can be updated individually, while being excluded from counts, batch updates and reminders. Uninstallation uses system confirmation and rescans installed packages after return.

- **后台更新与提醒**：默认每四小时处理模块、作用域和发现列表，有更新时通知；进入应用先显示可操作的缓存；已有待更新项时保留列表，无缓存或过期时按现有策略补全，普通返回前台不重复刷新。支持手动刷新和独立关闭，不自动下载或安装；系统可能延后任务，强行停止后需重新打开域见。<br>
  **Background refresh and reminders:** Refresh module, scope and Discover lists every four hours by default and notify about updates. Open actionable cached lists immediately. Retain lists with pending updates and fill missing or expired caches under the existing refresh policy; ordinary resumes do not repeat refreshes. Refresh manually or disable background checks separately. No automatic downloads or installation; Android may delay jobs, and ScopeView must be reopened after force stop.
- **配置备份**：在扳手中导出和导入用户设置、排序、收藏、忽略更新和自定义来源，包含有效默认值；不复制 Root、作用域、安装任务、APK 或目录缓存。<br>
  **Configuration backup:** Export and import user settings, sort order, bookmarks, ignored modules and custom sources, including effective defaults. Root state, scopes, installation tasks, APKs and catalog caches are excluded.
- **后台恢复**：可控制开机恢复与进程退出后的后台恢复，不自动弹出界面；系统限制及主动强行停止仍按 Android 行为处理。<br>
  **Background recovery:** Control boot restoration and recovery after process exit without opening a screen; Android restrictions and user force-stop remain respected.
- **Material 3 Expressive**：提供浅色和深色界面，保留固定标题栏与自然滚动；大列表分帧更新，重建界面后恢复滚动位置。<br>
  **Material 3 Expressive:** Light and dark interfaces retain the fixed toolbar and natural scrolling. Large lists update across frames and restore their scroll position after recreation.

## 使用要求 / Requirements

- Android 13 或更高版本。<br>
  Android 13 or later.
- 使用 LSPosed，并允许域见读取已安装应用列表。<br>
  Use LSPosed and allow ScopeView to access the installed app list.
- 读取作用域、读取 LSPosed 本机仓库缓存及直接安装更新需要 Root 授权；更新目录也会从官方公开源刷新。<br>
  Root authorization is required to read scopes and LSPosed's local repository cache and to install updates directly; the catalog also refreshes from the public official source.

## 作用域 / Scope

作用域仅声明域见自身（`io.github.zhongjitianqianguai.scopeview`），无需勾选其他应用。<br>
The scope declaration only lists ScopeView itself (`io.github.zhongjitianqianguai.scopeview`); no other apps need to be selected.

Xposed 入口仅在域见主进程加载时写一条框架日志，不拦截应用行为；读取配置和更新模块仍通过 Root 完成，无需激活该模块。<br>
The Xposed entry only writes a framework log when ScopeView's main process loads and does not intercept app behavior; configuration reads and module updates still use Root and do not require module activation.

## 开始使用 / Getting started

1. 打开域见，尚未授权时每次启动主动尝试一次 Root 申请，也可使用明确的授权按钮手动重试。授权后读取本机作用域；应用列表受限时，可用 Root 补充当前用户的模块识别。<br>
   Open ScopeView for one proactive Root request per launch while permission is missing, or retry with the explicit grant button. After authorization, read local scopes; Root can supplement module discovery for the current user when the ordinary app list is restricted.
2. 在应用列表中搜索目标应用，查看关联模块。<br>
   Search for an app in the app list to see its associated modules.
3. 进入应用先显示缓存；点击“刷新全部”统一扫描模块、读取作用域并检查更新，也可在“发现”中刷新目录。后台自动刷新默认开启，可在扳手中关闭。<br>
   Open cached lists first. Refresh all scans modules, reads scopes and checks updates together; Discover can refresh its catalog separately. Background refresh is enabled by default and can be disabled in Settings.
4. 切换到模块更新列表，选择单个更新、勾选后“更新所选”或“更新全部”。<br>
   Switch to the module update list to update one module, use Update selected or Update all.
5. 更新检查沿用管理器的来源和通道，兼容 Vector 的“仅正式版 / 包含预发布版”；联网失败时保留可用缓存。<br>
   Update checks follow the Manager’s source and channel, including Vector’s stable-only and prerelease-inclusive modes, and retain usable cached results when requests fail.

6. 打开“发现”，按最近更新或新收录浏览；展开摘要，收藏感兴趣的模块，或进入详情查看 README、历史版本和下载链接。<br>
   Open Discover to browse recent updates or new listings, expand previews, bookmark interesting modules or open details for the README, history and download links.

## 使用说明 / Usage notes

域见只读显示作用域，不修改 LSPosed 配置。<br>
ScopeView displays scopes without modifying the LSPosed configuration.

已读取的关联会保存在域见本地；在管理器中取消勾选后，仍显示为“对此应用已停用”，并与模块总开关状态分开。未曾读取且已删除的关联无法还原，未安装或未识别模块仍隐藏。<br>
Associations already read are saved locally in ScopeView. After deselection in the Manager, they remain visible as disabled for that app, separately from the module switch. Deleted associations never read cannot be recovered; uninstalled or unrecognized modules remain hidden.

后台检查只发出提醒，下载和安装必须由你主动发起；Beta、Nightly 和多 APK 版本需要你选择，稳定版单 APK 可加入更新队列。<br>
Background checks only send reminders; downloads and installation require your explicit action; choose Beta, Nightly and multi-APK releases, while a stable release with one APK can enter the update queue automatically.

安装前会核验包名与版本，并保留 Android 的签名和兼容性检查。<br>
Package names and versions are verified before installation, while Android retains its signature and compatibility checks.

Root 安装失败时，可将已验证的 APK 交给系统安装器。<br>
If Root installation fails, the verified APK can be handed to the system installer.

作用域记录保留 Android 用户 ID，应用名称和已安装状态按当前用户显示。<br>
Scope records retain Android user IDs, while app names and installation status are resolved for the current user.

Android 的同包 APK 由多个用户共享，因此更新模块也会更新其他已安装该模块的用户所使用的程序代码。<br>
Android shares package code across users, so updating a module also updates the code used by other users who have that package installed.
