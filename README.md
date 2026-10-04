# 域见 ScopeView

一眼看清哪些 LSPosed 模块作用于某个应用，不用再逐个点开查找。<br>
See at a glance which LSPosed modules target an app, without opening them one by one.

集中查看模块更新，支持单个更新和批量更新。<br>
Check module updates in one place and update them individually or in a batch.

[项目仓库 / Repository](https://github.com/Xposed-Modules-Repo/io.github.zhongjitianqianguai.scopeview) · [发布版本 / Releases](https://github.com/Xposed-Modules-Repo/io.github.zhongjitianqianguai.scopeview/releases)

## 主要功能 / Features

- **按应用查看模块**：查看一个应用被哪些模块选入作用域，显示应用名称、包名、图标及 Android 用户信息。<br>
  **Modules by app:** See which modules include an app in their scopes, with app names, package names, icons and Android user information.
- **查看模块更新**：读取 LSPosed 管理器的本机仓库缓存，显示缓存时间、更新标记和可更新数量。<br>
  **Check module updates:** Read the LSPosed Manager's local repository cache and show its timestamp, update indicators and available update count.
- **优先显示更新**：有更新的模块始终排在前面，各组内保留你选择的排序规则。<br>
  **Updates first:** Modules with available updates always appear first, with your chosen sort order preserved within each group.
- **单个或批量更新**：支持更新单个模块或“更新全部”，遇到多个 APK 时由你逐项选择或跳过。<br>
  **Individual or batch updates:** Update one module or use Update all, choosing or skipping each release that offers multiple APKs.
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

域见自身不 Hook 任何应用，无需勾选作用域；它展示的是其他模块为应用配置的作用域。<br>
ScopeView does not hook apps or require scope selection; it shows the scopes configured by other modules.

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

更新必须由你主动发起，多 APK 版本不会自动选择变体。<br>
Updates require your explicit action, and APK variants are never selected automatically.

安装前会核验包名与版本，并保留 Android 的签名和兼容性检查。<br>
Package names and versions are verified before installation, while Android retains its signature and compatibility checks.

Root 安装失败时，可将已验证的 APK 交给系统安装器。<br>
If Root installation fails, the verified APK can be handed to the system installer.

作用域记录保留 Android 用户 ID，应用名称和已安装状态按当前用户显示。<br>
Scope records retain Android user IDs, while app names and installation status are resolved for the current user.

Android 的同包 APK 由多个用户共享，因此更新模块也会更新其他已安装该模块的用户所使用的程序代码。<br>
Android shares package code across users, so updating a module also updates the code used by other users who have that package installed.
