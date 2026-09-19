# FrameCurator

更新发布通道：更新清单 + Windows x64 下载包（FrameCurator）。

- 当前版本：**1.0.0.30**（build 30）
- 最近更新：HEIC 解码组件改为独立 DLL 随包分发(许可合规),包内新增第三方许可声明;报告页新增文件名搜索/只看已勾选/反向选择/按组筛选/组号点击跳转/大库分页;主界面取消按钮空闲提示与打开报告降级提示;删除勾选显示逐张进度。

## 下载

| 用途 | 文件 |
|---|---|
| 首次安装（推荐，双击即装） | [FrameCurator-1.0.0.30-thirdparty-sources.zip](https://github.com/xmuhl-tools/FrameCurator-updates/releases/download/v1.0.0.30/FrameCurator-1.0.0.30-thirdparty-sources.zip) |
| 便携版 / 自动更新载荷 | [FrameCurator-1.0.0.30-win-x64.zip](https://github.com/xmuhl-tools/FrameCurator-updates/releases/download/v1.0.0.30/FrameCurator-1.0.0.30-win-x64.zip) |

## 安装与使用

- **安装包**：双击运行 → 确认/修改安装位置（默认 `%USERPROFILE%\FrameCurator`）→ 自动创建桌面快捷方式。
  程序与数据（配置、模板、日志、输出）都放在安装目录内；卸载 = 删除安装目录与快捷方式，不写注册表。
- **便携版**：把 exe 放进任意可写目录直接运行；配置与数据保存在程序目录的子目录内。

## 校验（sha256）

```text
FrameCurator-1.0.0.30-win-x64.zip
  1d7ef0172730c2dfdbe431cc423903647f19e65dc41c7117e7e5b4c70e52e67f
FrameCurator-1.0.0.30-thirdparty-sources.zip
  450b97404336124f7bf40063a8338a6a7514f3c5c53c2c8a6dfeaa9ede74b754
```

## 自动更新

程序启动时会读取本仓库的更新清单 [`update.json`](update.json)（镜像通道见清单内 `mirrors`），
按 build 号比较；发现新版本时提示下载，校验 sha256 后自动替换并重启。手动检查入口在程序主界面。

---
本文件由发布流程自动生成/更新（portable-app-release 技能，2026-09-19），请勿手工改动。
