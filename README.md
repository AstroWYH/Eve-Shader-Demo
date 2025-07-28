# 【UE5 C++】渲染 Shader 一个工程搞懂

![动画](https://github.com/user-attachments/assets/41f50ce6-6431-4a42-9390-5e93013d3f5a)

## 项目简介

本仓库对应B站视频[【UE5 C++】渲染 Shader 一个工程搞懂](https://www.bilibili.com/video/BV1siAkeFE4z/?spm_id_from=333.788.videopod.sections&vd_source=ab67845b846f1632f14b7e2c4a6c5935)的完整实现工程。视频聚焦UE5中基于C++的渲染Shader开发，适合有一定基础、尤其是在大型团队中需要更高自由度进行渲染相关工作的开发者，通过一个工程全面解析Shader开发的关键类、核心流程及实现逻辑。

## 核心内容

视频及配套工程主要围绕以下方面展开：

1. **Shader开发基础**

- 介绍UE5中Shader开发的文件形式（.usf文件），并与OpenGL的GLSL、DirectX的HLSL等进行类比，帮助开发者理解不同环境下Shader开发的差异。
- 明确顶点着色器（VS）和像素着色器（PS，UE5中常用称呼，类似其他环境中的片元着色器FS）在渲染流程中的核心作用。

2. **关键类与流程解析**

- 详细讲解与渲染Shader相关的重要类，梳理从代码编写到效果呈现的关键流程，包括如何将指令提交到渲染线程执行等核心环节。
- 解析渲染Pass的实现模板，从`BeginRenderPass`到`EndRenderPass`的完整过程，以及`SetGraphicsPipelineState`等常用接口的使用。

3. **代码与关联逻辑**

- 提供完整的.usf文件Shader代码示例，包含顶点着色器和像素着色器的具体实现。
- 说明自定义Shader类与Global Shader类的继承关系，以及如何将Shader类与.usf文件关联，指定VS和PS的对应关系。
- 讲解如何向Shader中传递参数，实现参数对渲染效果的动态影响。

## 工程获取与使用

1. **环境要求**

- Unreal Engine 5.0+
- 支持UE5 C++开发的IDE（如Visual Studio 2022、Rider等）

2. **下载地址**

- 完整工程：可在视频评论区获取，或访问[作者仓库](https://github.com/AstroWYH)相关项目（Eve-Shader-Demo、Eve-Render-Demo等私有项目）

3. **快速启动**
   获取工程后，右键`.uproject`文件选择对应UE5引擎版本，生成项目文件，编译后运行即可查看Shader渲染效果，可通过调整暴露的参数直观感受对渲染结果的影响。

## 适用人群

- 需进行UE5复杂渲染效果开发的开发者
- 大型游戏团队中负责渲染模块的程序人员
- 希望深入理解UE5渲染管线及Shader开发的学习者
- 有OpenGL、DirectX等Shader开发基础，想迁移到UE5的开发者

## 相关资源

- 视频链接：[【UE5 C++】渲染 Shader 一个工程搞懂](https://www.bilibili.com/video/BV1.../?spm_id_from=333.788.videopod.sections&vd_source=ab67845b846f1632f14b7e2c4a6c5935)
- 系列教程：作者其他UE5 C++教程（蓝图/C++对照、背包系统、网络同步等）
- 辅助工具：推荐使用RenderDoc等软件辅助调试Shader
- 参考项目：UE5官方渲染相关项目及作者推荐的GAS、Mass框架等学习项目

## 作者信息

前华为/百度程序员，专注分享UE5 C++游戏开发实战知识。

- 更多工程与源码：[个人仓库](https://github.com/AstroWYH)
- B站主页：[晚上做游戏](https://space.bilibili.com/89037636?spm_id_from=333.1007.0.0)

## 许可证

本工程基于MIT许可证开源，允许个人与商业项目自由使用、修改和分发，如需二次发布请注明原作者及视频来源。
