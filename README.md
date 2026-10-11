# 拉群小助手 · 桌面版

私域拉群进度管理工具（Windows 桌面版）。

## 下载

- **下载页**：https://cvrtgbp2dn-code.github.io/lq-helper/
- **所有版本**：https://github.com/cvrtgbp2dn-code/lq-helper/releases

## 自动更新

程序本体是一个 HTML 文件，**首次安装后不需要再下安装包**：

- 每次启动会静默检查 `app/version.json`
- 有新版就自动下载 `app/index.html`（131 KB，秒完成）并替换本地缓存
- 断网时用本地缓存，不影响使用

> 所以以后升级工具，只需要替换 `app/index.html` + 改一下 `app/version.json` 的版本号。

## 目录

| 路径 | 说明 |
|---|---|
| `index.html` | 下载页 |
| `app/index.html` | 程序本体（自动更新的目标） |
| `app/version.json` | 版本号，用来比对是否需要更新 |

## 数据

全部数据存在用户本机（Electron 的 localStorage / IndexedDB），不上传任何服务器。
换电脑用「数据备份 → 导出/恢复」。
