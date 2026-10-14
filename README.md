# 风月 · 发布仓库

这里发布风月的安装包与更新清单。本仓库只存放发布产物，不包含源码。

## 下载

请到 [Releases](https://github.com/Oranges-sama/FengYue-Releases/releases) 页面下载：

| 平台 | 文件 | 说明 |
|---|---|---|
| Windows | `FengYue-x.y.z-N-Setup.exe` | 双击安装 |
| Android | `FengYue-x.y.z-N-arm64-v8a.apk` | 绝大多数机型都是这个（体积也最小）|

## 更新清单

`latest.json` 是软件内置更新器的入口，记录当前版本、各文件的 SHA-256 与下载地址。

```
https://raw.githubusercontent.com/Oranges-sama/FengYue-Releases/main/latest.json
```

国内直连不稳定时，走镜像前缀即可（如 `https://gh-proxy.com/<上面的地址>`）。


## 版本号

形如 `1.0.11+4`：前半是显示版本，`+N` 是构建号（只增不减）。

## 文档

- [使用说明](docs/USAGE.md)
- [专业版说明](docs/PRO.md)
- [更新清单字段说明](docs/MANIFEST.md)

## 反馈

遇到问题、或者想要新功能，都欢迎到 [Issues](../../issues) 里说。点「New issue」会看到对应的模板，照着填就行。

提问题时顺手写上版本号（软件「设置 → 关于」里能看到），能省不少来回。
