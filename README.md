# 风月 FengYue · 发布仓库

> 本仓库**只放发布产物与更新清单**，不含源码。

## 目录约定

| 文件 | 用途 |
|---|---|
| `latest.json` | ⭐ **更新清单**：版本号、安装包/APK/产物文件的 sha256、附件地址 |
| `latest-beta.json` | （预留）测试通道 |

安装包、APK、差分补丁等**大文件**放在 [Releases](../../releases) 附件里，**不进本仓库** ✗。

## 更新器怎么用

```
GET https://raw.githubusercontent.com/Oranges-sama/FengYue-Releases/main/latest.json
```

`latest.json` 字段（详见 `docs/更新与分发方案.md` §1.3）：

```json
{
  "channel": "stable",
  "version": "1.0.11",
  "build": 4,
  "versionCode": 4,
  "appVersion": "1.0.11+4",
  "publishedAt": "2026-10-14T05:00:00Z",
  "notes": "",
  "installer": { "name": "风月-1.0.11-4-安装包.exe", "size": 0, "sha256": "…", "url": "" },
  "apks": [ { "name": "风月-1.0.11-4-all.apk", "size": 0, "sha256": "…", "url": "" } ],
  "files": [ { "path": "fengyue_media.exe", "size": 0, "sha256": "…" } ]
}
```

⛔ **`files` 只含「普通版」产物**；管理员版是内部变体，**不发布** ✗。
