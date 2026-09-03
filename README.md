<div align="center">

# 🧑‍💼 员工关系 ER 工作台

**面向 HRBP 的员工关系事项总览、Case 管理与方案执行工作台**

*Employee Relations Workbench — 让分散的员工关系事项，收敛成一条清晰可执行的工作闭环。*

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)](https://developer.mozilla.org/zh-CN/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)](https://developer.mozilla.org/zh-CN/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=000)](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript)
[![GitHub Pages](https://img.shields.io/badge/Deploy-GitHub%20Pages-222?style=flat-square&logo=github&logoColor=white)](https://pages.github.com/)
[![零后端](https://img.shields.io/badge/架构-零后端-2ea44f?style=flat-square)](./)
[![零依赖](https://img.shields.io/badge/依赖-零框架-blue?style=flat-square)](./)

**单文件 · 零后端 · 本地数据存储 · 无需 API Key**

</div>

---

## 📑 目录

- [项目简介](#-项目简介)
- [核心能力](#-核心能力)
  - [HRBP 工作台总览](#1-hrbp-工作台总览)
  - [Case 管理](#2-case-管理)
  - [方案与执行闭环](#3-方案与执行闭环)
  - [Excel 与本地数据](#4-excel-与本地数据)
- [技术特点](#-技术特点)
- [快速开始](#-快速开始)
- [部署到 GitHub Pages](#-部署到-github-pages)
- [项目结构](#-项目结构)
- [数据与隐私](#-数据与隐私)
- [使用边界](#-使用边界)
- [贡献与反馈](#-贡献与反馈)
- [许可说明](#-许可说明)

---

## 🎯 项目简介

**员工关系 ER 工作台**是一套面向 **HRBP** 的轻量级员工关系管理界面，帮助团队集中处理部门内部的员工关系事项，并把「**事项概览 → 风险识别 → Case 建立 → 推荐方案 → 任务执行 → 文书草稿**」组织成一条清晰的工作闭环。

本项目采用**纯 HTML / CSS / JavaScript** 实现，具备三个关键特征：

| 特征 | 说明 |
| --- | --- |
| ⚡ **零后端** | 无需数据库服务、无需服务器、无需 API Key |
| 🔒 **本地优先** | 新增事项、方案选择、任务状态与文书草稿默认保存在浏览器 `localStorage` |
| 🚀 **即开即用** | 可直接双击打开，也可一键部署为 GitHub Pages 静态站点 |

适合作为**可直接分发的内部工具原型**、**方案演示项目**或 **GitHub Pages 静态站点**。

> 💡 当前登录身份展示为 **ZOE｜HRBP**；界面不包含任何具体公司名称。

---

## 🛠️ 核心能力

整个工作台围绕一条闭环展开：

```mermaid
flowchart LR
    A[📋 事项概览] --> B[🚨 风险识别]
    B --> C[📁 Case 建立]
    C --> D[🧭 推荐方案]
    D --> E[✅ 任务执行]
    E --> F[📝 文书草稿]
    F -. 复盘 .-> A
```

### 1. HRBP 工作台总览

一眼掌握部门员工关系全貌：

- ✅ 待办事项与临期提醒；
- 📊 Case 处理流程看板；
- 🎯 高 / 中 / 低风险分布；
- 📈 任务完成率、待处理 Case、执行中 Case 的平滑趋势图；
- 🔍 知识库快捷问答入口。

### 2. Case 管理

内置 8 类常见员工关系事项：

| 事项类型 | 事项类型 |
| --- | --- |
| 📉 绩效改进（PIP） | 🤝 协商解除 |
| 🏥 工伤处理 | ⚖️ 部门冲突与申诉 |
| 💰 加班费争议 | ⚠️ 纪律与行为问题 |
| 🤰 三期员工管理 | 📄 合同到期不续签 |

### 3. 方案与执行闭环

每个 Case 自动匹配一套「方案—执行—文书」链路：

- **方案 A（推荐）/ 方案 B / 方案 C** 三条处理路径对比；
- 各方案的**适用情况、行动建议、优势、主要风险、可行性**说明；
- 可推进的任务清单：`待开始 → 进行中 → 已完成`；
- 匹配事项类型的**文书草稿入口**；
- **本地规则建议助手**：生成 HRBP 初步行动建议与升级边界提醒。

### 4. Excel 与本地数据

- 📥 下载标准 Excel 导入模板；
- 📤 浏览器本地导入 `.xlsx` / `.csv` 事项数据；
- 📊 导出当前事项为 Excel；
- 💾 导出 / 恢复 JSON 本地备份；
- 🕐 自动展示 `Asia/Shanghai` 中国标准时间。

---

## 🧰 技术特点

| 分类 | 说明 |
| --- | --- |
| **前端** | 原生 HTML、CSS、JavaScript，无框架依赖 |
| **图表** | 内置 SVG 平滑趋势图、科技渐变环形图 |
| **数据存储** | 浏览器 `localStorage` |
| **Excel** | 纯前端生成 / 解析 `.xlsx` 与 `.csv` |
| **部署** | 可直接双击打开；也可使用 GitHub Pages 托管 |
| **外部服务** | 默认不调用任何外部 API，也不需要 API Key |

---

## 🚀 快速开始

### 方式一：直接打开

下载或克隆本仓库后，直接用浏览器打开：

```bash
index.html
```

推荐浏览器：**Chrome** 或 **Edge**。

### 方式二：使用本地静态服务（推荐）

在项目目录中执行：

```bash
python3 -m http.server 8080
```

然后访问：

```text
http://127.0.0.1:8080
```

> 💡 使用本地静态服务可避免部分浏览器对本地文件导入、下载或存储行为的限制。

---

## 🌐 部署到 GitHub Pages

本项目是静态单页应用，仓库根目录已有 `index.html`，可直接发布。

1. 将本项目推送到 GitHub 的 `main` 分支；
2. 进入仓库的 **Settings → Pages**；
3. 在 **Build and deployment** 中配置：
   - **Source**：`Deploy from a branch`
   - **Branch**：`main`
   - **Folder**：`/ (root)`
4. 点击 **Save**；
5. 等待发布完成后访问：

```text
https://<你的GitHub用户名>.github.io/<仓库名>/
```

以仓库名 `employee-relations-workbench` 为例：

```text
https://<你的GitHub用户名>.github.io/employee-relations-workbench/
```

---

## 📂 项目结构

```text
employee-relations-workbench/
├── index.html          # 完整工作台：界面、样式、图表与交互逻辑
├── README.md           # 项目说明与部署文档
├── .gitignore          # Git 忽略规则
└── .nojekyll           # 防止 GitHub Pages 执行 Jekyll 处理
```

---

## 🔒 数据与隐私

本项目使用浏览器 `localStorage` 保存数据，这意味着：

- 数据只保存在**当前浏览器与当前域名**下；
- GitHub Pages 访问者彼此的数据互不共享；
- 清除浏览器站点数据后，本地事项也会被清除；
- 使用「系统管理 → 导出 JSON 备份」可迁移或备份数据；
- 项目默认不会将事项数据发送到第三方服务。

### ⚠️ 重要提醒

员工关系信息通常具有敏感性，请务必：

- **不要**将真实员工姓名、医疗信息、绩效记录、投诉材料或沟通纪要提交到公开 GitHub 仓库；
- 若项目将用于内部真实业务，请创建 **Private Repository（私有仓库）**；
- 若需要多人共享数据、权限管理、审计日志或服务端 AI 能力，请使用独立的后端版本，而不要将敏感数据存入静态站点源码。

---

## ⚖️ 使用边界

本项目提供的本地规则建议、推荐方案和文书草稿，仅用于辅助 HRBP 进行事项梳理与执行组织，**不构成法律、医疗或专业意见**。

在涉及员工权益、敏感身份、工伤、三期员工、解除 / 不续签、纪律处理或高风险争议时，应按照公司制度、适用规则及内部审批机制处理，并由 ER 专家、HRD 或其他有权角色进行复核。

---

## 🤝 贡献与反馈

欢迎通过 Issue 或 Pull Request 提出：

- 🎨 交互与视觉优化建议；
- 📋 Case 类型与方案模板扩展；
- 📊 Excel 字段与导入规则改进；
- 🧭 HRBP 工作流、风险提示和文书模板建议。

---

## 📜 许可说明

当前仓库**未附带开源许可证**。如计划公开开源，请根据实际使用场景选择合适的许可证（例如 MIT、Apache-2.0 或私有许可）。

---

<div align="center">

**Made with ❤️ for HRBP**

*让员工关系事项，处理得更专业、更有条理。*

</div>
