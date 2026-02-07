# Lubrication Coating Research Skills

## 润滑涂层材料学术研究技能工具包

---

## 项目简介 | Project Overview

A collection of Claude Code skills for academic research workflows in lubrication coating materials science. This toolkit is designed to help researchers write literature reviews, prepare coating synthesis reports, design experiments, and generate research proposals in the field of tribology and surface engineering.

面向润滑涂层材料科学领域的 Claude Code 学术研究技能工具包。该工具包帮助研究者撰写文献综述、制备涂层合成报告、设计实验方案、生成研究计划书，涵盖摩擦学与表面工程全流程。

## Skills | 技能

| Skill | Description | 描述 | Trigger / 触发词 |
|-------|-------------|------|-----------------|
| [tribology-review](./tribology-review/) | Write comprehensive literature reviews for lubrication coatings | 撰写润滑涂层综合文献综述 | `/tribology-review`, "tribology review", "coating review", "摩擦学综述", "涂层综述" |
| [coating-synthesis-review](./coating-synthesis-review/) | Review coating deposition and synthesis methods | 综述涂层沉积与制备方法 | `/coating-synthesis`, "coating preparation", "PVD CVD", "制备方法综述" |
| [research-proposal](./research-proposal/) | Generate PhD research proposals for tribology research | 生成摩擦学研究博士研究计划 | `/tribology-proposal`, "research proposal", "PhD proposal", "研究计划" |
| [tribology-testing](./tribology-testing/) | Generate tribological testing reports | 生成摩擦学测试报告 | `/tribology-testing`, "wear testing", "摩擦学测试" |

## Features | 功能特点

### tribology-review
- **7阶段工作流** | 7-phase systematic workflow
- **涂层分类指南** | Coating category guidelines (DLC, MoS₂, WS₂, etc.)
- **摩擦学指标库** | Tribological metrics database (COF, wear rate, hardness)
- **多源文献搜索** | Multi-source literature integration

### coating-synthesis-review
- **制备方法综述** | Deposition method reviews (PVD, CVD, Thermal Spray)
- **工艺参数优化** | Process parameter optimization strategies
- **表征方法指南** | Characterization techniques guide

### research-proposal
- **中英双语支持** | Bilingual support (EN/ZH)
- **Nature Reviews风格** | Nature Reviews-style academic writing
- **多文献源整合** | Multi-source literature integration

### tribology-testing
- **ASTM/ISO标准** | Testing standards reference (ASTM G99, ISO 20808)
- **测试设备指南** | Equipment guide (Pin-on-disk, 4-ball, etc.)
- **数据分析方法** | Data analysis methodology

## Installation | 安装

### 全局安装 | Global Installation

```bash
# 克隆仓库
git clone https://github.com/your-username/lubrication-coating-skills.git

# 复制到 Claude Code 技能目录
cp -r tribology-review ~/.claude/skills/
cp -r coating-synthesis-review ~/.claude/skills/
cp -r research-proposal ~/.claude/skills/
cp -r tribology-testing ~/.claude/skills/
```

### 项目本地安装 | Project-Local Installation

```bash
cp -r tribology-review .agents/skills/
cp -r coating-synthesis-review .agents/skills/
cp -r research-proposal .agents/skills/
cp -r tribology-testing .agents/skills/
```

## MCP Configuration | MCP 配置

### 必需 MCP 服务器 | Required MCP Servers

本工具包需要配置以下 MCP 服务器以获得最佳体验：

This toolkit requires the following MCP servers for optimal experience:

```bash
# ArXiv MCP Server - 用于搜索最新材料科学研究
# For searching latest materials science research
npm install -g arxiv-mcp-server

# Scholar MCP Server - 用于 Google Scholar 文献搜索
# For Google Scholar literature search
npm install -g scholar-mcp-server
```

详细配置说明请参考 | See detailed setup instructions:
- [tribology-review/references/MCP_SETUP.md](./tribology-review/references/MCP_SETUP.md)
- [research-proposal/references/LITERATURE_WORKFLOW.md](./research-proposal/references/LITERATURE_WORKFLOW.md)

## Usage | 使用示例

### tribology-review | 撰写润滑涂层综述

```
/tribology-review
我想写一篇关于"DLC涂层摩擦学性能"的文献综述
```

### coating-synthesis-review | 综述涂层制备方法

```
/coating-synthesis-review
请帮我写一篇关于"PVD涂层制备工艺"的综述文章
```

### research-proposal | 生成研究计划

```
/tribology-proposal
我需要一个关于"高温自润滑涂层"的博士研究计划
```

### tribology-testing | 生成测试报告

```
/tribology-testing
帮我生成一份"DLC涂层耐磨性能测试"的实验报告模板
```

## Project Structure | 项目结构

```
lubrication-coating-skills/
├── README.md
├── LICENSE
├── tribology-review/
│   ├── SKILL.md
│   └── references/
│       ├── WORKFLOW.md
│       ├── DOMAINS.md
│       ├── METRICS.md
│       ├── LITERATURE_SOURCES.md
│       ├── TEMPLATES.md
│       ├── QUALITY_CHECKLIST.md
│       └── MCP_SETUP.md
├── coating-synthesis-review/
│   ├── SKILL.md
│   └── references/
│       ├── WORKFLOW.md
│       ├── DEPOSITION_METHODS.md
│       ├── PARAMETER_OPTIMIZATION.md
│       ├── CHARACTERIZATION.md
│       └── QUALITY_CHECKLIST.md
├── research-proposal/
│   ├── SKILL.md
│   ├── references/
│   │   ├── STRUCTURE_GUIDE.md
│   │   ├── WRITING_STYLE_GUIDE.md
│   │   ├── LITERATURE_WORKFLOW.md
│   │   └── QUALITY_CHECKLIST.md
│   └── assets/
│       ├── proposal_scaffold_en.md
│       └── proposal_scaffold_zh.md
└── tribology-testing/
    ├── SKILL.md
    └── references/
        ├── WORKFLOW.md
        ├── TESTING_STANDARDS.md
        ├── EQUIPMENT.md
        └── DATA_ANALYSIS.md
```

## Supported Domains | 支持的研究领域

### 涂层类型 | Coating Types
- 固体润滑涂层 | Solid lubricant coatings (MoS₂, WS₂, h-BN, Graphene)
- 类金刚石涂层 | Diamond-like carbon (DLC)
- 金属基自润滑涂层 | Metal-based self-lubricating coatings
- 陶瓷涂层 | Ceramic coatings (TiN, CrN, Al₂O₃)
- 多层/纳米复合涂层 | Multilayer/nanocomposite coatings

### 应用领域 | Application Areas
- 航空航天 | Aerospace components
- 汽车工业 | Automotive parts
- 切削工具 | Cutting tools and molds
- 生物医疗 | Biomedical implants
- 海洋工程 | Marine engineering

## License | 许可证

MIT License

Copyright (c) 2024 Lubrication Coating Research Skills

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

## Citation | 引用

If you use this toolkit in your research, please cite:

```
Lubrication Coating Research Skills. (2024). A collection of Claude Code skills
for academic research in tribology and surface engineering. GitHub repository.
```

## Contributing | 贡献指南

欢迎提交 Issue 和 Pull Request 来改进此工具包。

Issues 和 PR 请遵循以下规范：
1. 使用中英双语描述问题
2. 提供具体的使用场景
3. 附上相关错误信息（如有）

## Contact | 联系方式

For questions or suggestions, please open an Issue on GitHub.

---

**Happy Research! | 研究愉快!**
