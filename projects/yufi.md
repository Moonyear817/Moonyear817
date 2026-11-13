# Yufi · 桌面助手

[返回主页](../README.md) · [GitHub 源码](https://github.com/Moonyear817/Yufi) · [上游 Dela](https://github.com/Chang-Yo/Dela)

基于 Dela 改造的本地优先桌面助手，将 Canvas 课程资料、课堂录音转写、项目文件与内置终端放在同一个工作台。

**工具**　Electron · React · TypeScript · sherpa-onnx · SenseVoice · Qwen3-ASR

## 制作过程

### 从现有工作台开始

保留 Dela 的 Electron 工作台与 Pi Agent 内核，围绕实际使用场景改造课程与笔记流程；隐藏不适用的课表、课堂视频与社区入口。

### Canvas 会话登录

用应用内登录窗口与会话 Cookie 替代手动填写访问令牌，调整学期名称识别，连接课程资料预览与下载。登录和课程同步已做本地验证。

### 本机录音与双阶段转写

按课程管理录音，SenseVoice 提供实时预览，Qwen3-ASR 完成分句转写。修复 Electron 模块加载与 WebM 时长元数据，让回放能显示时长并拖动定位；已测试中英文录音和回放。

### 当前状态

macOS 内置终端已适配。Microsoft 365 OAuth 代码已接入，实际邮箱权限仍待管理员批准；AI 整理笔记和远程 SSH 尚待实际验证。仓库提供开发源码，暂未发布 Yufi 安装包。

## 来源与许可

Yufi 是 [Dela](https://github.com/Chang-Yo/Dela) 的衍生改造，沿用 GPL-3.0-or-later 许可；桌面框架与 Agent 能力来自上游项目。

---

A local-first desktop assistant adapted from Dela, combining Canvas materials, lecture recording and transcription, local files and a terminal. Sign-in, transcription and audio playback were tested locally. Microsoft 365 mail needs administrator approval; AI note organization and remote SSH remain unverified. Source code is available; no Yufi installer has been published.
