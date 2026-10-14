# 风月 · 发布仓库

这里发布风月的安装包与更新清单。本仓库只存放发布产物，不包含源码。

## 下载

请到 [Releases](https://github.com/Oranges-sama/FengYue-Releases/releases) 页面下载：

| 平台 | 文件 | 说明 |
|---|---|---|
| Windows | `风月-x.y.z-N-安装包.exe` | 双击安装 |
| Android | `风月-x.y.z-N-all.apk` | 不确定机型就选这个 |
| Android | `风月-x.y.z-N-<架构>.apk` | 明确架构时选，体积更小 |

## 更新清单

`latest.json` 是软件内置更新器的入口，记录当前版本、各文件的 SHA-256 与下载地址。

```
https://fastly.jsdelivr.net/gh/Oranges-sama/FengYue-Releases@main/latest.json
```

字段说明与整体方案见 [docs/更新与分发方案.md](https://github.com/Oranges-sama/FengYue/blob/main/docs/更新与分发方案.md)。

## 版本号

形如 `1.0.11+4`：前半是显示版本，`+N` 是构建号（只增不减）。

## 反馈

遇到问题、或者想要新功能，都欢迎到 [Issues](../../issues) 里说。点「New issue」会看到对应的模板，照着填就行。

提问题时顺手写上版本号（软件「设置 → 关于」里能看到），能省不少来回。
