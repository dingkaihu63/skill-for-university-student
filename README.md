# 思政论文 skill



# 🎓 Sizheng Writer: 高校思政论文全栈写作重构方案

[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Python](https://img.shields.io/badge/python-3.8%2B-blue.svg)](https://www.python.org/)
[![Claude](https://img.shields.io/badge/Claude-Skill%20Compatible-purple.svg)](https://www.anthropic.com/claude)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/dingkaihu63/skill-for-university-student/pulls)

**Sizheng Writer** 是一款专为大学生设计的“Claude Code Skill”工具集。它不仅能辅助生成思政论文、心得体会、实践报告，更通过**四维去AI化重构引擎**与**AIGC概率自检协议**，确保文本具备真实的认知轨迹、严谨的理论支撑与个性化的表达风格。

---

## ✨ 核心特性

| 模块 | 功能描述 | 技术实现 |
| :--- | :--- | :--- |
| **重构引擎** | 强制句法熵增，消除 AI 均匀感 | `rewrite-standards.md` |
| **权威对齐** | 实时校准 30+ 官方政务资料源 | `official-sources.json` |
| **自检审计** | 模拟算法进行四维 AIGC 概率评估 | `aigc-detection-framework.md` |
| **自动排版** | 一键导出符合学术规范的 `.docx` | `generate_docx.py` |

---

## 📂 项目结构

```text
.
├── SKILL.md                   # 核心系统指令集 (System Prompt)
├── rewrite-standards.md       # 深度重构与去AI化执行标准
├── aigc-detection-framework.md # 四维 AIGC 检测评估框架
├── official-sources.json      # 权威政务与理论参考索引
├── generate_docx.py           # 自动化学术文档生成脚本
└── README.md                  # 项目说明文档
````

-----

## 🚀 快速上手

### 1\. 导入 Skill

将 `SKILL.md` 中的全部内容复制，粘贴至 **Claude 3.5 Sonnet / Opus** 的对话框或设置为自定义 Skill。

### 2\. 环境配置 (用于本地导出)

若需使用自动排版功能，请确保安装 Python 依赖：

```bash
pip install python-docx
```

### 3\. 标准工作流

1.  **意图识别**：告知主题、字数及目标检测率（如：\< 15%）。
2.  **逻辑建构**：Claude 将根据 `official-sources.json` 提供理论框架。
3.  **文本生成**：执行“去模板化”写作，植入“初识-深入-内化”认知轨迹。
4.  **自检报告**：自动调用 `aigc-detection-framework.md` 进行压力测试。
5.  **本地导出**：获取生成的 JSON 内容，运行 `generate_docx.py` 即可在桌面获得成品。

-----

## 🛠️ 技术深度

### 去 AI 化语言学策略 (Linguistic Strategy)

不同于简单的同义词替换，本项目执行以下底层策略：

  - **句法抖动**：强制 3:2 的长短句分布，打破生成模型常见的 1:1 机械平衡。
  - **语态转换**：将 80% 的被动语态转化为“认知主体+主动动词”结构。
  - **细节锚定**：在案例描述中强制要求时间、地点、调研对象等高颗粒度细节。

-----

## ⚖️ 免责声明

1.  **学术诚信**：本工具仅用于学术表达优化及辅助排版，使用者应对论文内容的真实性及学术合规性负全部责任。
2.  **政治立场**：所有输出内容必须严格遵守所在国家法律法规，确保政治立场绝对正确。
3.  **算法局限**：AIGC 检测评分基于概率模型，不代表真实查重系统的最终结果。

-----

## 🤝 贡献与反馈

如果你有新的权威资料源或更优的重写规则，欢迎提交 Pull Request。

  - **Author**: [dingkaihu63](https://www.google.com/search?q=https://github.com/dingkaihu63)
  - **Repo URL**: [dingkaihu63/skill-for-university-student](https://www.google.com/search?q=https://github.com/dingkaihu63/skill-for-university-student)

