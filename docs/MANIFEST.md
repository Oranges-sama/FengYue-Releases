# 更新清单字段说明（latest.json）

本文件说明 `latest.json` 的字段口径。软件启动后会读取它来判断是否有新版本。

## 顶层字段

| 字段 | 含义 |
|---|---|
| `channel` | 发布通道，目前固定 `stable` |
| `version` | 版本号，形如 `1.0.12` |
| `build` | 构建号，**单调递增**，同版本号下用它判断新旧 |
| `appVersion` | 完整版本，形如 `1.0.12+5`（显示时会写成 `1.0.12-5`）|
| `versionCode` | 安卓 `versionCode` |
| `tag` | 对应的 Release 标签，形如 `v1.0.12-5` |
| `notes` | **本版本的更新说明**（Markdown 原文）|
| `notesUrl` | 说明的网页地址 |
| `installer` | Windows 安装包（见下）|
| `apks` | Android 安装包列表 |
| `mirrors` | 备用下载地址（节点/镜像）|
| `files` | 文件清单与校验值（供完整性校验使用）|

## installer / apks 里的字段

| 字段 | 含义 |
|---|---|
| `name` | 文件名（**ASCII** ✓）|
| `size` | 字节数 |
| `sha256` | 文件校验值，下载后软件会核对 |
| `url` | 下载地址（GitHub Releases 附件）|
| `localName` | 本地打包时的原始文件名（仅备查）|

## 更新判断规则

1. 先比 `version`（逐段数字比较）；
2. 版本号相同时再比 `build`，`build` 更大即为更新。

## 怎么访问

```
https://raw.githubusercontent.com/Oranges-sama/FengYue-Releases/main/latest.json
```

国内直连不稳定时，软件会自动走内置加速节点（如 `gh-proxy.com`）。
