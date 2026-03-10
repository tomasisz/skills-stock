# 🚀 Stock Analyzer: 基于 Gemini CLI 的深度股票分析引擎

[![Gemini CLI](https://img.shields.io/badge/Powered%20by-Gemini%20CLI-blue)](https://github.com/google/gemini-cli)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**Stock Analyzer** 是一个高度集成的智能分析工具，运行于 [Gemini CLI](https://github.com/google/gemini-cli) 环境。它将复杂的投资银行分析框架转化为自动化的 AI 工作流，为个人投资者提供机构级的深度研究报告。

---

## ✨ 核心特性

本工具通过 `stock-analyzer` 技能实现，核心优势包括：

*   **🏛️ 机构级分析框架**：严格遵循高盛、摩根士丹利等顶级投行的研究逻辑。
*   **🧠 深度护城河评估**：不仅看财报，更深度挖掘品牌、技术专利、网络效应等“隐形资产”，并给出 1-10 的量化评分。
*   **📊 动态财务扫描**：自动调取并分析过去 5 年的营收、毛利、债务及 ROE 趋势。
*   **📉 多维度估值模型**：结合行业市盈率（P/E）对比与贴现现金流（DCF）估算。
*   **⚔️ 逻辑辩论赛**：自动模拟“牛市分析师”与“熊市分析师”的数据对垒，助你识别认知的盲区。
*   **📰 实时财报拆解**：针对最新季度财报，分析预期差及市场情绪。

---

## 🛠️ 快速安装

### 1. 环境准备
确保您的系统中已安装并配置好 [Gemini CLI](https://github.com/google/gemini-cli)。

### 2. 下载仓库
```bash
git clone https://github.com/tomasisz/skills-stock.git
cd skills-stock
```

### 3. 配置技能 (Skill)
将技能定义文件同步到 Gemini CLI 的配置目录：
```bash
# 创建技能目录
mkdir -p ~/.gemini/skills/stock-analyzer

# 复制技能定义
cp SKILL.md ~/.gemini/skills/stock-analyzer/
```

---

## 💡 使用指南

启动 Gemini CLI 后，您可以使用以下方式获取深度分析：

### 🔹 自然语言触发
您可以像咨询私人分析师一样提问：
*   `分析股票 特斯拉`
*   `帮我拆解一下 NVIDIA 的财务健康状况`
*   `分析 TSLA 的护城河评分是多少？`

### 🔹 显式激活模式
在复杂对话中，建议先激活技能以进入“专家模式”：
```bash
/activate_skill stock-analyzer
```

---

## 📖 报告结构预览

生成的每一份报告都包含以下标准模块：
1.  **商业模式与收入来源** (Business Model)
2.  **竞争优势评估** (Moat Analysis & Scoring)
3.  **财务健康度审计** (Financial Health Check)
4.  **投行估值分析** (Valuation: P/E & DCF)
5.  **核心风险排序** (Risk Matrix)
6.  **多空逻辑辩论** (Bull vs Bear Debate)
7.  **最终投资策略** (Final Verdict: Buy/Hold/Avoid)

---

## 📂 核心文件说明

*   **`SKILL.md`**: 核心逻辑定义，包含了 AI 的角色设定、工作流及输出规范。
*   **`README.md`**: 项目导航手册（即本文件）。
*   **`Google Gemini analyze stock.md`**: 原始分析模板，可作为手动分析的参考。

---

## 🤝 贡献与反馈
欢迎通过 Issue 提交功能建议，或通过 Pull Request 贡献更多的分析维度（如 ESG 评分、宏观相关性等）。

## ⚠️ 投资免责声明
**本工具生成的分析内容仅供学习与研究参考，不构成任何形式的投资建议。** 市场有风险，投资需谨慎。在做出任何金融决策前，请咨询专业的金融顾问并进行独立的调查。

---
*Generated & Maintained with ❤️ by Gemini CLI*
