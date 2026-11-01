<div align="center">

# Meguvizarchic

[![项目](https://img.shields.io/badge/%E9%A1%B9%E7%9B%AE-12-00AEEC?style=flat-square&labelColor=2d3a55)](https://github.com/orgs/Meguvizarchic/repositories)
[![平台](https://img.shields.io/badge/Android-8.1%2B-2d3a55?style=flat-square&labelColor=2d3a55)](#项目一览)
[![Maven](https://img.shields.io/badge/groupId-io.github.jichuo1.meguviz-FB7299?style=flat-square&labelColor=2d3a55)](#项目一览)

### 面向 Android 与原生计算的 Meguviz 系列基础库

</div>

---

## 简介

Meguvizarchic 收纳了 **Meguviz** 系列项目与凝光视效引擎。每个项目都可以独立构建、独立使用，不要求同时引入系列中的其他项目；项目之间通过**可选桥接**协作，默认关闭，按需接入。

> [!NOTE]
> 已正式发布：MeguvizRef、MeguvizUI、MeguvizAndroid、MeguvizDrawable、凝光视效引擎。其余项目仍在开发中，接入前请阅读各仓库的状态说明。

---

## 项目一览

### 🧩 Android 基础

| 项目 | 说明 | 状态 |
| --- | --- | --- |
| [MeguvizRef](https://github.com/Meguvizarchic/MeguvizRef) | 面向 Java 17 与 Android 的反射工具库，通过描述符精确定位方法、字段与构造器，并以作用域统一管理加载器与缓存、以独立于接收对象的调用计划完成可复用的调用 | `1.0.0` · Central |
| [MeguvizAndroid](https://github.com/Meguvizarchic/MeguvizAndroid) | 为 Android 应用提供生命周期、窗口、资源加载与有界调度能力的基础库，各模块可按需组合接入 | `1.0.0` · GitHub |
| [MeguvizHook](https://github.com/Meguvizarchic/MeguvizHook) | 拥有自有 API 与执行核心的独立 Android Hook SDK，通过可切换的 libxposed 101 / 102 后端完成方法拦截，并为每一项安装结果提供清晰回执 | 开发中 |

### 🎨 界面与视觉

| 项目 | 说明 | 状态 |
| --- | --- | --- |
| [MeguvizUI](https://github.com/Meguvizarchic/MeguvizUI) | 面向 Android 原生 View 的强类型 Kotlin UI 库，在编译期约束布局结构，并以属性所有权与会话生命周期管理界面状态的每一次更新 | `1.0.0` · Central |
| [凝光视效引擎](https://github.com/Meguvizarchic/LumenCoacervationEngine) | 面向 Android View 系统的可移植玻璃材质与视效引擎，为卡片、悬浮栏、弹窗和页面提供随设备能力自动适配的柔光与高级材质以及丰富的交互动效 | `1.6.1` · JitPack |
| [MeguvizDrawable](https://github.com/Meguvizarchic/MeguvizDrawable) | 以不可变绘制配方描述形状、颜色、渐变与描边的 Android Drawable 库，配合形状 provider 与有界单飞缓存 `FlightCache`，并可按需桥接 Compose、MeguvizAndroid、MeguvizUI 与 Lumen | `1.0.0` · Central |

### ⚙️ 原生计算与媒体

| 项目 | 说明 | 状态 |
| --- | --- | --- |
| [MeguvizMemory](https://github.com/Meguvizarchic/MeguvizMemory) | 提供显式 CPU 内存域与有界 arena 的内存管理库，以读写分离的 lease 和分阶段关闭流程保证所有权清晰与资源安全回收 | 工程预览 |
| [MeguvizCompute](https://github.com/Meguvizarchic/MeguvizCompute) | 基于固定版本 ncnn 构建的计算 SDK，以版本化的纯 C ABI 和有界任务模型为上层算法统一提供运行时、资源与调度能力 | 开发 SDK |
| [MeguvizShaderTools](https://github.com/Meguvizarchic/MeguvizShaderTools) | 独立的着色器主机工具 `mgst`，在锁定的工具链下完成 GLSL 编译、SPIR-V 校验与布局反射，并打包为可复现的不可变 shaderpack | 候选版本 |
| [MeguvizRIFE](https://github.com/Meguvizarchic/MeguvizRIFE) | 基于 MeguvizCompute 的 RIFE 插帧算法库，支持 v4.6 模型并通过纯 C 接口为宿主提供帧间插值能力 | 开发 SDK |
| [MeguvizMedia](https://github.com/Meguvizarchic/MeguvizMedia) | 集帧与时间线核心、公开 C ABI、可选 RIFE 适配与 Android JNI 库于一体的媒体处理框架，为插帧与图像处理流程提供统一的时序与资源管理 | 开发 SDK |

### 🔍 分析工具

| 项目 | 说明 | 状态 |
| --- | --- | --- |
| [MeguvizDexDash](https://github.com/Meguvizarchic/MeguvizDexDash) | 面向桌面与云端、可嵌入也可服务化的 DEX 静态分析引擎，为 APK 与 DEX 提供带来源身份的结构检查与分析能力 | 开发中 |

---

## 许可证

各项目分别授权，以对应仓库的 `LICENSE` 为准。

| 许可证 | 项目 |
| --- | --- |
| Apache-2.0 | MeguvizRef、MeguvizUI、MeguvizAndroid、MeguvizDrawable、MeguvizHook、凝光视效引擎 |
| MIT | MeguvizCompute、MeguvizShaderTools |
| GPL-3.0 | MeguvizRIFE、MeguvizMedia |

## 致谢

感谢 ncnn、Xposed / LSPosed 社区，以及参与测试和反馈的用户。

如果这些项目对你有帮助，欢迎通过 Issue 提交可复现的问题或改进建议。
