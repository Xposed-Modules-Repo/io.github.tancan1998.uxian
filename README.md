# U 闲

闲鱼净化与增强模块，包名 `io.github.tancan1998.uxian`，需要兼容 libxposed API 102 的框架。

功能：开屏及部分信息流广告过滤、消息与入口整理、首页导航与金刚位排序、任务执行计划和进度，以及可选调试和临时抓包。功能独立开关，按实际钩子挂载情况报告适配。

## 源码、AI 声明与开源协议

主要代码、文档、测试和构建配置由 AI（OpenAI ChatGPT / Codex，通过 Minis）生成并迭代，由维护者提出需求、审核和提供实测反馈。

- 完整源码：https://github.com/TanCan1998/uxian
- 下载：https://github.com/Xposed-Modules-Repo/io.github.tancan1998.uxian/releases
- 协议：GNU GPL v3.0（GPL-3.0-only）
- 许可证原文：https://github.com/TanCan1998/uxian/blob/main/LICENSE
- 第三方版权及许可证：https://github.com/TanCan1998/uxian/blob/main/NOTICE.md

特别感谢芝麻粒 M（aw1y2z/Sesame-M）的 RPC 通道、任务过滤、失败黑名单和调度参考；感谢其上游 Dragon813/Sesame-GR、SenOffical/Sesame-TK、constanline/XQuickEnergy、pansong291/XQuickEnergy，以及相关维护者和贡献者。完整来源、许可证和致谢保留在源码仓库。本项目并非上述项目的官方版本。

## 已实测宿主与验证边界

闲鱼 **7.28.91 / versionCode 529**：维护者于 2026-11-06 确认当前已安装版本全部现有功能正常；历史亦验证过 7.28.80 / 525。公开版已清空旧代码中的精确位置默认值，依赖位置的任务和本次包名迁移尚未重新进行真机验证。契约测试、云端构建和静态检查不替代新的真机验收。

临时抓包与报告可能包含当前账户的请求、响应或身份信息，分享前需脱敏。HTTP 调试默认关闭，仅绑定本机回环且未设置鉴权，请仅调试时启用。

## 从旧包名迁移

新版包名为 `io.github.tancan1998.uxian`，旧包名为 `com.xiandehuang.u`。请先停用旧模块，再安装并启用新模块、设置闲鱼作用域后重启宿主，避免重复 Hook。本次发行没有自动替换设备上已安装的模块。

本仓库只分发模块说明和 APK，完整对应源码与许可证见上方链接。
