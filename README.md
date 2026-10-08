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
  如果域见对你有帮助，欢迎点一个 Star 支持项目 ⭐
  <br>
  If ScopeView helps you, please consider leaving a Star.
</p>

<p align="center">
  <a href="https://github.com/Xposed-Modules-Repo/io.github.zhongjitianqianguai.scopeview/releases">公开下载 / Downloads</a> · <a href="https://github.com/Xposed-Modules-Repo/io.github.zhongjitianqianguai.scopeview">官方索引 / Official index</a>
</p>

## 主要功能 / Features

- **按应用查看模块**：查看一个应用被哪些模块选入作用域，显示应用名称、包名、图标及 Android 用户信息。<br>
  **Modules by app:** See which modules include an app in their scopes, with app names, package names, icons and Android user information.
- **查看模块更新**：读取 LSPosed 管理器的仓库缓存，跟随其更新通道，显示缓存时间并识别仅名称变化的版本更新。<br>
  **Check module updates:** Read the LSPosed Manager's repository cache, follow its selected channel, show the cache timestamp and recognize updates that only change the version name.
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

## 使用要求 / Requirements

- Android 13 或更高版本。<br>
  Android 13 or later.
- 使用 LSPosed，并允许域见读取已安装应用列表。<br>
  Use LSPosed and allow ScopeView to access the installed app list.
- 读取作用域、读取 LSPosed 仓库缓存及直接安装更新需要 Root 授权。<br>
  Root authorization is required to read scopes and the LSPosed repository cache, and to install updates directly.

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
5. 仓库信息较旧时，先在 LSPosed 管理器中刷新仓库，再回到域见刷新。<br>
   If the repository data is outdated, refresh it in LSPosed Manager, then refresh ScopeView.

## 使用说明 / Usage notes

域见只读显示作用域，不修改 LSPosed 配置。<br>
ScopeView displays scopes without modifying the LSPosed configuration.

更新必须由你主动发起；Beta、Nightly 和多 APK 版本需要你选择，稳定版单 APK 可加入更新队列。<br>
Updates require your explicit action; choose Beta, Nightly and multi-APK releases, while a stable release with one APK can enter the update queue automatically.

安装前会核验包名与版本，并保留 Android 的签名和兼容性检查。<br>
Package names and versions are verified before installation, while Android retains its signature and compatibility checks.

Root 安装失败时，可将已验证的 APK 交给系统安装器。<br>
If Root installation fails, the verified APK can be handed to the system installer.

## 本次更新 / What's new in 0.0.3

- 新增模块更新日志展开与收起，支持 Markdown 显示；官方模块按需读取日志，自定义来源保留发布说明。<br>
  Expand or collapse module changelogs with Markdown rendering; official notes load on demand and custom sources retain release descriptions.
- 补充 LSPosed 寄生管理器和秘密代码备用入口，保留独立管理器跳转；备用入口打开首页时会给出提示。<br>
  Add parasitic-manager and secret-code fallback routes while retaining standalone-manager navigation, with a notice when a fallback opens the home page.
- 在设置的“日志与诊断”中导出并分享诊断日志，记录管理器打开、读取、下载、安装等关键步骤。<br>
  Export and share diagnostic logs from Logs and diagnostics in Settings, including key manager, read, download and installation steps.
- 增加帧耗时、长帧、布局与绘制、界面任务墙钟/CPU 耗时及内存信息，方便排查卡顿。<br>
  Add frame timing, slow-frame, layout and draw, UI task wall/CPU timing, and memory information to help investigate lag.
- 整理设置页面，加入官方交流群、发布频道和项目 Star 入口，更新返回箭头；日志导出使用明确的文字按钮。<br>
  Organize Settings with the official group, release channel and project Star links, update the back arrow, and use a clearly labeled log-export button.
- 调整长截图相关布局：标题栏下全部内容统一滚动，详情与设置共用外层 ScrollView；分别保存页面位置并复用未变化的卡片。<br>
  Adjust the layout for scrolling screenshots: all content below the toolbar scrolls together, details and Settings share the outer ScrollView, and page positions and unchanged cards are retained.

项目地址：[域见 ScopeView](https://github.com/Xposed-Modules-Repo/io.github.zhongjitianqianguai.scopeview)，欢迎点一个 Star 支持项目 ⭐<br>
Project: [ScopeView](https://github.com/Xposed-Modules-Repo/io.github.zhongjitianqianguai.scopeview). Please consider leaving a Star if it helps you.

## 本次更新 / What's new in 0.0.4

- 修复寄生管理器模式读取 LSP 仓库缓存时提示“未找到仓库缓存”的问题，补充当前用户的宿主缓存路径，保留独立管理器支持。<br>
  Fix repository-cache lookup in parasitic-manager mode by adding the current user's host cache path while retaining standalone-manager support.
- 独立与寄生缓存都存在时，读取更新较新的一份，并使用同一来源的更新通道，保留 Stable、Beta 和 Nightly 行为。<br>
  When both caches exist, read the newer one and its matching update channel, preserving Stable, Beta and Nightly behavior.
- 增加缓存探测与选择日志，记录来源、时间和通道，方便排查读取问题；管理器文件保持只读。<br>
  Add cache-probe and selection logs with the source, timestamp and channel to help diagnose read issues; Manager files remain read-only.
