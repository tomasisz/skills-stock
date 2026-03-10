# Stock Analyzer (股票深度分析专家) 📈

本项目是一个基于 [Gemini CLI](https://github.com/google/gemini-cli) 的自定义技能（Skill），旨在通过 AI 动力为投资者提供专业、详尽、数据驱动的股票深度分析报告。

## 🌟 核心功能

本项目集成的 `stock-analyzer` 技能遵循投资银行（如高盛、摩根士丹利）的专业分析框架，涵盖以下维度：

- **商业模式拆解**：深入分析公司的收入来源与运作逻辑。
- **竞争优势评估（护城河）**：从品牌、网络效应、转换成本等维度评估，并给出 1-10 的专业评分。
- **财务健康度扫描**：分析过去 5 年的营收增长、利润率、债务水平及 ROE。
- **投资银行级估值**：包含市盈率（P/E）行业对比及贴现现金流（DCF）估算。
- **多空对垒辩论**：模拟两位持有不同观点（看多 vs 看空）的分析师进行数据支撑的辩论。
- **财报实时解读**：分析最新季度财报表现及市场反应。
- **最终投资建议**：提供短期及长期的明确投资结论。

## 🚀 安装与设置

### 前提条件
- 已安装并配置好 [Gemini CLI](https://github.com/google/gemini-cli)。
- 拥有 Google Gemini API Key。

### 技能配置步骤

1. **克隆仓库**：
   ```bash
   git clone https://github.com/您的用户名/skills-stock.git
   ```

2. **同步技能文件**：
   将 `SKILL.md` 文件链接或复制到您的 Gemini CLI 技能目录中：
   ```bash
   mkdir -p ~/.gemini/skills/stock-analyzer
   cp SKILL.md ~/.gemini/skills/stock-analyzer/
   ```

## 💡 如何使用

在终端启动 Gemini CLI 后，您可以直接通过自然语言触发分析：

### 示例指令：
- `分析 NVIDIA (NVDA)`
- `给我一份关于 特斯拉 (TSLA) 的深度研究报告`
- `深度拆解 阿里巴巴 (BABA) 的竞争护城河`

### 显式激活技能：
如果您希望手动确保加载此框架，可以输入：
```
/activate_skill stock-analyzer
```

## 📂 目录结构

- `Google Gemini analyze stock.md`: 原始分析模板及参考文档。
- `SKILL.md`: Gemini CLI 技能定义文件，包含核心逻辑与系统指令。
- `README.md`: 项目使用说明。

## ⚠️ 免责声明

本工具生成的分析报告仅供参考，不构成任何投资建议。投资有风险，入市需谨慎。在使用 AI 生成的数据进行决策前，请务必咨询专业金融顾问。

---
*由 Gemini CLI 自动生成与维护*
