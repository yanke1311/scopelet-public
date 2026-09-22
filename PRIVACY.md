# Scopelet privacy notice

Applies to Scopelet 0.1.10. Publisher: `ke-yan` (display name `ke.yan`).

## English

### Files and queries

Scopelet reads files in the search scope you choose and processes queries, filenames, paths, matching text, and preview contents. A preview may read unsaved text from an open editor. Processing happens in the VS Code extension host: on the local machine for a local workspace, or in the workspace's remote environment when using a remote host such as WSL. File/text search uses the bundled ripgrep executable; syntax highlighting uses bundled code and WebAssembly in the webview. Scopelet does not execute the source code being previewed or automatically save your edits.

### Saved state and controls

Search history can contain query text, directory paths, glob patterns, relative-path bases and search options. Scope history stores groups of directories/globs and their base; it remains compatible with earlier directory history. Search history and scope history each retain up to 20 entries in VS Code workspace state. Scopelet also stores search options and preview preferences. These values are not encrypted by Scopelet and are subject to access controls, backups and retention of the host environment. There is no automatic time-based expiry: older history entries are evicted as new entries are added, or you can clear them. Closing the panel does not clear saved workspace state. Without an open workspace, this state is kept in memory for the extension-host session.

Use the Command Palette to run:

- **Scopelet: Clear Search History** — clear saved searches.
- **Scopelet: Clear Directory History** — clear saved scope groups and earlier directory history.
- **Scopelet: Clear Workspace History** — clear both histories.
- **Scopelet: Reset Preview Preferences** — reset saved preview preferences.

Clearing histories does not reset search options or preview preferences and does not erase backups or third-party logs. Queries are passed to ripgrep as process arguments and may be visible to local process-inspection or diagnostic tools according to host permissions. Avoid searching for secrets if you do not want them exposed this way or retained in a subsequently saved search.

### Network and third parties

Scopelet does not include analytics, advertising, a developer-operated backend, or a feature that uploads your queries or file contents to the publisher. Normal installed use does not collect or write Scopelet performance timing logs. Automated Test mode can record timing diagnostics for development; test tools and their output should not be used with sensitive fixtures.

Symbol/reference searches invoke your installed language extensions through VS Code APIs. Those extensions may use their own language servers or remote services. Remote workspace transport and storage are provided by VS Code and the remote environment. Their behavior is governed by their own configuration and policies; this notice is not a promise that every component of your editor works offline.

Marketplace/documentation pages display images hosted on GitHub. When you view them, the hosting services may receive normal web-request information, such as your IP address and browser details, under their policies. These page requests are separate from Scopelet's file-search processing.

### Support and questions

[GitHub Issues](https://github.com/yanke1311/scopelet-public/issues) is the public support channel. If you submit an issue, the maintainer and other visitors can see your GitHub identity and the content you choose to post. Provide only redacted, non-sensitive examples. GitHub controls storage and retention on its service. For privacy questions, open an issue containing only the question, not the sensitive data; if private evidence is needed, arrange an appropriate channel before sending it.

## 简体中文

### 文件与查询

Scopelet 读取你选择的搜索范围，处理查询、文件名、路径、命中文本和预览内容；预览可能读取编辑器中尚未保存的文字。处理发生在 VS Code 扩展宿主：本地工作区在本机，WSL 等远端工作区在相应远端环境。文件/文本搜索使用随包提供的 ripgrep，高亮使用随包提供的代码和 WebAssembly。插件不会执行被预览的源码，也不会自动保存你的修改。

### 保存的数据与控制方式

搜索历史可能包含查询文本、目录路径、glob、相对路径基准和选项。范围历史保存目录/glob 组合及其基准，并兼容旧目录历史。搜索历史、范围历史各自在 VS Code 工作区状态中最多保留 20 条；另外保存搜索选项和预览偏好。Scopelet 不自行加密这些数据，访问权限、备份和存储保留受宿主环境控制。没有按时间自动过期的机制：新增历史会挤出最旧的条目，也可以手动清理。关闭面板不会清除已保存的工作区状态。没有打开工作区时，这些状态仅保留在当前扩展宿主会话的内存中。

通过命令面板可执行 **Scopelet: Clear Search History**、**Clear Directory History**、**Clear Workspace History** 清除对应历史；**Reset Preview Preferences** 重置预览偏好。清除历史不会重置搜索选项或预览偏好，也不会删除环境备份或第三方日志。查询会作为进程参数传给 ripgrep，可能被符合宿主权限的本地进程检查或诊断工具看到。不希望敏感内容以此方式暴露或进入后续保存的搜索记录时，请避免用它作为查询。

### 网络与第三方

Scopelet 没有内置分析统计、广告、开发者运营的后端，也没有将查询或文件内容上传给发布者的功能。正常安装使用不采集或写入性能计时日志；自动化 Test 模式可以记录开发用计时，测试工具与输出应使用非敏感样本。

符号和引用搜索通过 VS Code API 调用已安装的语言扩展，它们可能使用自己的语言服务器或远程服务。远端工作区的通信和存储由 VS Code 及远端环境提供，其行为受各自配置与政策约束，不能因此承诺整个编辑器及所有组件都不联网。

Marketplace 和文档页面会显示 GitHub 托管的图片。访问这些页面时，托管服务可能依其政策获取 IP 地址、浏览器信息等正常网页请求数据；这与插件处理文件搜索是不同的数据路径。

### 支持与隐私问题

[GitHub Issues](https://github.com/yanke1311/scopelet-public/issues) 是公开支持渠道。提交 Issue 后，维护者和其他访问者可以看到你的 GitHub 身份及主动提交的内容，请只使用脱敏的非敏感示例。GitHub 控制其服务的数据存储与保留。隐私问题可先通过 Issue 说明问题本身，不要贴出敏感数据；需要提供私有证据时，先商定适当渠道。
