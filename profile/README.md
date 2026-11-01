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
| [MeguvizRef](https://github.com/Meguvizarchic/MeguvizRef) | 反射工具库：描述符精确查询、作用域生命周期、与接收对象解耦的调用计划，核心零第三方依赖 | `1.0.0` · Central |
| [MeguvizAndroid](https://github.com/Meguvizarchic/MeguvizAndroid) | 生命周期、窗口、资源与有界调度基础库 | `1.0.0` · GitHub |
| [MeguvizHook](https://github.com/Meguvizarchic/MeguvizHook) | 独立 Hook SDK：自有 API 与执行核心，libxposed 101 / 102 后端互斥，安装结果逐项回执 | 开发中 |

### 🎨 界面与视觉

| 项目 | 说明 | 状态 |
| --- | --- | --- |
| [MeguvizUI](https://github.com/Meguvizarchic/MeguvizUI) | 原生 View 强类型 Kotlin UI 库：编译期布局约束、属性所有权、会话生命周期 | `1.0.0` · Central |
| [凝光视效引擎](https://github.com/Meguvizarchic/LumenCoacervationEngine) | 可移植玻璃材质与视效引擎：柔光 / 高级材质按设备自动降级，附带可选动效模块 | `1.6.1` · JitPack |
| [MeguvizDrawable](https://github.com/Meguvizarchic/MeguvizDrawable) | Drawable 库：不可变绘制配方、形状 provider 与有界单飞缓存 `FlightCache`，可选 Compose、Android、UI 与 Lumen 桥接 | `1.0.0` · Central |

### ⚙️ 原生计算与媒体

| 项目 | 说明 | 状态 |
| --- | --- | --- |
| [MeguvizMemory](https://github.com/Meguvizarchic/MeguvizMemory) | 显式 CPU 内存域与有界 arena，读写 lease 分离，分阶段关闭 | 工程预览 |
| [MeguvizCompute](https://github.com/Meguvizarchic/MeguvizCompute) | 基于固定版本 ncnn 的计算 SDK：版本化 C ABI、有界任务、唯一 ncnn owner | 开发 SDK |
| [MeguvizShaderTools](https://github.com/Meguvizarchic/MeguvizShaderTools) | `mgst` 着色器工具：GLSL 编译、SPIR-V 校验与反射、不可变 shaderpack | 候选版本 |
| [MeguvizRIFE](https://github.com/Meguvizarchic/MeguvizRIFE) | RIFE 插帧算法库，支持 v4.6 模型与纯 C 接口 | 开发 SDK |
| [MeguvizMedia](https://github.com/Meguvizarchic/MeguvizMedia) | 帧与时间线 core、C ABI、可选 RIFE 适配与 Android JNI 库 | 开发 SDK |

### 🔍 分析工具

| 项目 | 说明 | 状态 |
| --- | --- | --- |
| [MeguvizDexDash](https://github.com/Meguvizarchic/MeguvizDexDash) | 面向桌面与云端、可嵌入且可服务化的 DEX 静态分析引擎 | 开发中 |

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
