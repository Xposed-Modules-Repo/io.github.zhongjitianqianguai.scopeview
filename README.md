# 域见 ScopeView

按应用反查 LSPosed 模块作用域，集中查看和管理模块更新。

[项目仓库](https://github.com/Xposed-Modules-Repo/io.github.zhongjitianqianguai.scopeview) · [发布版本](https://github.com/Xposed-Modules-Repo/io.github.zhongjitianqianguai.scopeview/releases)

## 主要功能

- **查看作用域**：查看一个应用被哪些模块选入作用域，显示应用名称、包名、图标及 Android 用户信息。
- **查看模块更新**：读取 LSPosed 管理器的本机仓库缓存，显示缓存时间、更新标记和可更新数量。有更新的模块始终排在前面。
- **单个或批量更新**：支持更新单个模块或“更新全部”。遇到多个 APK 时，逐项选择需要的文件或跳过；取消剩余任务时会等待当前项完成。
- **搜索与排序**：应用、模块和作用域详情可以独立排序，保存已选规则；支持按名称或包名搜索。
- **中英界面**：默认跟随系统语言，也可手动选择简体中文或英文。
- **跳转管理器**：从模块详情打开 LSPosed 管理器中的对应模块。

## 使用要求

- Android 13 或更高版本。
- 使用 LSPosed，并允许域见读取已安装应用列表。
- 读取作用域、读取 LSPosed 仓库缓存及直接安装更新需要 Root 授权。

域见是独立管理工具，不包含 Xposed Hook 入口，无需在 LSPosed 中为域见勾选作用域。

## 开始使用

1. 打开域见，点击“读取作用域”，按授权指引允许 Root。
2. 在应用列表中搜索目标应用，查看关联模块。首次成功读取后，应用启动或回到前台会自动刷新。
3. 切换到模块更新列表，选择单个更新或“更新全部”。多个 APK 不会自动选择变体。
4. 仓库信息较旧时，先在 LSPosed 管理器中刷新仓库，再回到域见刷新。

域见只读显示作用域，不修改 LSPosed 配置。更新必须由用户主动发起；安装前核验包名与版本，保留 Android 的签名和兼容性检查。Root 安装失败时，可将已验证的 APK 交给系统安装器。

作用域记录会保留 Android 用户 ID，应用名称和已安装状态按当前用户显示。Android 的同包 APK 由多个用户共享，更新模块也会更新其他已安装该模块的用户所使用的程序代码。

## English

ScopeView is a standalone companion app for inspecting LSPosed scopes by app and managing installed module updates.

- View which modules include an app in their configured scopes, with app names, package names, icons and Android user IDs.
- Compare installed versions with the LSPosed Manager's local repository cache. Modules with available updates always appear first.
- Update one module or run a sequential Update all queue. Choose or skip every multi-APK release; cancelling lets the current item finish before stopping the rest.
- Search and save independent sort preferences. Follow the system language or select Simplified Chinese or English.
- Open the selected module in LSPosed Manager.

Requires Android 13 or later. Root is needed to read scopes and the Manager repository cache, and to install updates directly. The first scope read requires an explicit action and authorization; after a successful read, returning to ScopeView refreshes the data. Refresh the repository in LSPosed Manager when its cache is outdated.

ScopeView does not edit LSPosed scopes or install updates automatically. Downloads are checked for package and version, and Android retains its signature and compatibility checks. The system installer remains available if direct Root installation fails. Android shares package code across users, so updating a module also updates the code used by other users who have that package installed.
