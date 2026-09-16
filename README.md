# FrameCurator 影选 — 发布通道

FrameCurator 影选是一个 Windows 本地照片智能筛选工具：递归扫描照片目录，在原图只读的前提下分析技术质量、审美、人物瞬间、重复、连拍与相似场景，组内竞争产出精选集，并生成 HTML / CSV / SQLite 报告与导出精选照片。

本仓库是它的更新发布通道，不是源码仓库：`update.json` 是更新清单（版本、SHA-256、镜像链，附 RSA-2048 签名），Releases 提供各版本安装包。

> Release 页的 "Source code (zip / tar.gz)" 是 GitHub 为标签自动生成的快照（无法关闭），不是安装包；请下载 Assets 区的 `FrameCurator-<版本>-win-x64.zip`。

## 下载

- 最新版本：https://github.com/xmuhl-tools/FrameCurator-updates/releases/latest
- 国内镜像（jsDelivr，同一文件）：https://cdn.jsdelivr.net/gh/xmuhl-tools/FrameCurator-updates@v1.0.0.19/FrameCurator-1.0.0.19-win-x64.zip

## 安装与使用

1. 解压 zip 到任意可写目录（绿色软件：不写注册表，配置与目录历史保存在程序目录内）；
2. 双击 `FrameCurator.exe`；
3. 填输入目录（照片所在）与输出目录（报告与导出结果），点「开始分析」；
4. AI 模型权重不入包：按 `MODEL_MANIFEST.json` 自行准入后 AI 相关评分才启用，缺权重时该项显示 MODEL_UNAVAILABLE，其余功能照常。

系统要求：Windows 10 / 11（x64）。

## 自动更新

程序启动时读取本仓库 `update.json` 检查更新：发现新版本弹窗提示（立即更新 / 跳过此版本 / 稍后）。更新清单带 RSA-2048 数字签名，客户端验证通过才会采信，签名缺失或验不过一律拒绝该通道；下载包强制 SHA-256 校验，通过并经确认后才替换并重启；任一步失败都不影响当前使用。

## 完整性校验

SHA-256 记录在 `update.json` 的 `sha256` 字段，可自行核对：`certutil -hashfile FrameCurator-<版本>-win-x64.zip SHA256`。
