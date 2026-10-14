<p align="center">
  <img src="assets/scopeview-logo.png" width="168" height="168" alt="域见 ScopeView icon">
</p>

<h1 align="center">域见 ScopeView</h1>

<p align="center">
  每次更新 LSP 模块都要一个个点进去下载，根本不清楚有多少模块同时作用于某个应用？我来帮你。
  <br>
  Updating LSP modules means opening each one to download, with no clear view of how many modules target the same app? I'm here to help.
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

- **按应用查看模块**：查看一个应用被哪些模块选入作用域，显示应用名称、包名、图标及 Android 用户信息。<br>
  **Modules by app:** See which modules include an app in their scopes, with app names, package names, icons and Android user information.
- **查看模块更新**：直接检查已安装模块的官方详情，并核对管理器缓存；沿用更新通道，失败时保留已有结果，识别仅名称变化的更新。<br>
  **Check module updates:** Check official details for installed modules and reconcile the Manager cache; follow the selected channel, retain existing results on failure and recognize version-name-only updates.
- **通知快捷入口**：默认开启，点击通知打开域见；授权 Root 和通知权限后，划掉后台仍保留入口，设置中可关闭并保存选择。<br>
  **Notification shortcut:** Enabled by default; tap to open ScopeView. With Root and notification permission granted, it remains after removing the app from Recents; turn it off in Settings with your choice saved.
- **优先显示更新**：有更新的模块始终排在前面，各组内保留你选择的排序规则。<br>
  **Updates first:** Modules with available updates always appear first, with your chosen sort order preserved within each group.
- **单个或批量更新**：支持更新单个模块或“更新全部”；Beta、Nightly 和多 APK 项目由你逐项选择或跳过，没有 APK 的更新需你确认跳过。<br>
  **Individual or batch updates:** Update one module or use Update all; choose or skip each Beta, Nightly, or multi-APK item, and explicitly skip updates with no APK.
- **取消剩余任务**：等待当前更新完成，再停止后续更新。<br>
  **Cancel remaining updates:** Let the current update finish, then stop the remaining items.
- **搜索与排序**：按名称或包名搜索，为应用、模块和作用域详情分别保存排序规则。<br>
  **Search and sort:** Search by name or package name and save separate sort preferences for apps, modules and scope details.
- **中英界面**：默认跟随系统语言，也可手动选择简体中文或英文。<br>
  **Chinese and English:** Follow the system language by default or choose Simplified Chinese or English manually.
- **跳转管理器**：从模块详情打开 LSPosed 管理器中的对应模块。<br>
  **Open in Manager:** Open the corresponding module in LSPosed Manager from its details.

- **模块日志与诊断**：展开或收起模块发布说明，支持 Markdown；在设置中导出诊断日志。<br>
  **Module notes and diagnostics:** Expand or collapse release notes with Markdown support and export diagnostic logs from Settings.

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

1. 打开域见，点击“读取作用域”，按授权指引允许 Root。<br>
   Open ScopeView, tap Read scopes and follow the guide to grant Root access.
2. 在应用列表中搜索目标应用，查看关联模块。<br>
   Search for an app in the app list to see its associated modules.
3. 首次成功读取后，应用启动或回到前台会自动刷新。<br>
   After the first successful read, scope data refreshes when ScopeView opens or returns to the foreground.
4. 切换到模块更新列表，选择单个更新或“更新全部”。<br>
   Switch to the module update list to update one module or use Update all.
5. 点击“刷新更新”获取官方目录；应用会沿用 LSPosed 管理器的通道，并在联网失败时显示可用缓存。<br>
   Tap Refresh updates to fetch the official catalog; ScopeView follows LSPosed Manager's channel and shows usable cached results if the request fails.

## 使用说明 / Usage notes

域见只读显示作用域，不修改 LSPosed 配置。<br>
ScopeView displays scopes without modifying the LSPosed configuration.

更新必须由你主动发起；Beta、Nightly 和多 APK 版本需要你选择，稳定版单 APK 可加入更新队列。<br>
Updates require your explicit action; choose Beta, Nightly and multi-APK releases, while a stable release with one APK can enter the update queue automatically.

安装前会核验包名与版本，并保留 Android 的签名和兼容性检查。<br>
Package names and versions are verified before installation, while Android retains its signature and compatibility checks.

Root 安装失败时，可将已验证的 APK 交给系统安装器。<br>
If Root installation fails, the verified APK can be handed to the system installer.
