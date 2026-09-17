# FrameCurator

更新发布通道：更新清单 + Windows x64 下载包（FrameCurator）。

- 当前版本：**1.0.0.25**（build 25）
- 最近更新：新增「更新」菜单:手动检查更新、跳过版本可恢复,代理网络也能收到更新;进度条全程平滑不再回跳卡顿;报告页错误提示全中文,页面刷新后给出重新进入指引;导出完成直接显示导出目录;命令行新增中文帮助、导出进度与取消;修复专业相机照片(大 ICC 配置文件)拍摄信息读取、GPS 越界容错、相册打包下载健壮性等。

## 下载

| 用途 | 文件 |
|---|---|
| 便携版 / 自动更新载荷 | [FrameCurator-1.0.0.25-win-x64.zip](https://github.com/xmuhl-tools/FrameCurator-updates/releases/download/v1.0.0.25/FrameCurator-1.0.0.25-win-x64.zip) |

## 校验（sha256）

```text
FrameCurator-1.0.0.25-win-x64.zip
  c8df4818ee8eeccf002454d2f80c845d5c3ee1897c409b71329946048c4f65ff
```

## 自动更新

程序启动时会读取本仓库的更新清单 [`update.json`](update.json)（镜像通道见清单内 `mirrors`），
按 build 号比较；发现新版本时提示下载，校验 sha256 后自动替换并重启。手动检查入口在程序主界面。

---
本文件由发布流程自动生成/更新（portable-app-release 技能，2026-09-17），请勿手工改动。
