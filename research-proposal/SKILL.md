---
name: tribology-research-proposal
description: >
  Generate high-quality academic research proposals for lubrication coating and tribology research.
  Use when writing PhD proposals, research plans, or project applications for coating materials research.
  Triggers on requests for "research proposal", "PhD proposal", "研究计划",
  "博士研究计划", or mentions of research planning, funding proposals in tribology domain.
metadata:
  author: user
  version: "1.0.0"
allowed-tools:
  - Read
  - Write
  - Edit
  - Glob
  - Grep
  - Bash
  - WebSearch
  - WebFetch
  - Task
  - mcp__arxiv-mcp-server__search_papers
  - mcp__arxiv-mcp-server__download_paper
  - mcp__scholar-mcp-server__search
  - mcp__scholar-mcp-server__get_paper_details
---

# Tribology Research Proposal Skill

## 摩擦学研究计划撰写技能

---

## Quick Start | 快速开始

1. **Gather requirements** (topic, domain, language, word count)
2. **Collect literature** from multiple sources
3. **Generate outline** for user approval
4. **Write full proposal** based on approved outline
5. **Output Markdown** with quality checklist

**See | 参见**: [references/LITERATURE_WORKFLOW.md](references/LITERATURE_WORKFLOW.md)

---

## Core Principles | 核心原则

### Writing Style | 写作风格

- **Nature Reviews style**: Prose-based, hedging language
- **Evidence-based**: Every claim needs support
- **Structured**: Clear sections with logical flow
- **Quantitative**: Specific metrics, timelines, budgets

### Proposal Structure | 提案结构

| Section | Purpose | Length |
|---------|---------|--------|
| Title | Clear, specific, impactful | - |
| Abstract | Summary of entire proposal | 250-300 words |
| Introduction | Background, significance, gap | 20% |
| Objectives | Specific, measurable goals | 10% |
| Methodology | Research approach | 25% |
| Expected Outcomes | Deliverables, impact | 10% |
| Timeline | Phases, milestones | 10% |
| References | Supporting literature | 30-50 |

---

## Standard Proposal Structure | 标准提案结构

```markdown
# [Title]: Research Proposal

## Abstract | 摘要

## 1. Introduction | 引言
### 1.1 Background | 背景
### 1.2 Significance | 研究意义
### 1.3 Research Gap | 研究空白

## 2. Research Objectives | 研究目标

## 3. Literature Review | 文献综述
### 3.1 [Topic 1]
### 3.2 [Topic 2]
### 3.3 [Topic 3]

## 4. Research Methodology | 研究方法
### 4.1 Approach | 研究方法
### 4.2 Materials and Methods | 材料与方法
### 4.3 Characterization | 表征方法
### 4.4 Data Analysis | 数据分析

## 5. Expected Outcomes | 预期成果

## 6. Timeline | 研究计划

## 7. Significance and Impact | 意义与影响

## 8. References | 参考文献
```

---

## Key Features | 主要特点

### 5-Phase Workflow | 五阶段工作流

| Phase | Task | Output |
|-------|------|--------|
| 1 | Requirements gathering | Project brief |
| 2 | Literature collection | Literature matrix |
| 3 | Outline development | Proposal outline |
| 4 | Content writing | Full proposal |
| 5 | Quality check | Final document |

### Multi-Source Integration | 多源整合

| Source | Best For | Tools |
|--------|----------|-------|
| ArXiv | Latest methods, ML | search_papers |
| Scholar | Broad coverage | search, get_paper_details |
| Web Search | Funding info | WebSearch |

---

## Bilingual Support | 双语支持

### Language Options | 语言选项

| Option | Use Case |
|--------|-----------|
| English | International journals, funding |
| Chinese | Domestic applications, 中文期刊 |
| Bilingual | Comparative studies |

### Output Formats | 输出格式

| Format | Application |
|--------|-------------|
| Markdown | Editable draft |
| Word (via pandoc) | Submission ready |
| PDF (via pandoc) | Final submission |

---

## Target Length | 目标长度

| Type | Target Words | Typical References |
|------|--------------|-------------------|
| PhD Proposal | 3000-5000 | 40-60 |
| Postdoc Proposal | 2000-3000 | 30-50 |
| Grant Application | 5000-10000 | 50-100 |
| Internal Proposal | 1500-2500 | 20-40 |

---

## Reference Files | 参考文件

| File | Purpose |
|------|---------|
| [references/STRUCTURE_GUIDE.md](references/STRUCTURE_GUIDE.md) | Section-by-section guide |
| [references/WRITING_STYLE_GUIDE.md](references/WRITING_STYLE_GUIDE.md) | Academic writing style |
| [references/LITERATURE_WORKFLOW.md](references/LITERATURE_WORKFLOW.md) | Literature collection |
| [references/QUALITY_CHECKLIST.md](references/QUALITY_CHECKLIST.md) | Quality verification |
| [assets/proposal_scaffold_en.md](assets/proposal_scaffold_en.md) | English template |
| [assets/proposal_scaffold_zh.md](assets/proposal_scaffold_zh.md) | Chinese template |

---

## Usage Examples | 使用示例

### Example 1 | 示例1

**User | 用户**:
```
/tribology-proposal
我需要一个关于"高温自润滑涂层"的博士研究计划，
英文，目标5000字，申请美国大学博士项目。
```

**System Response | 系统响应**:
1. Search ArXiv for latest high-temp coating research
2. Search Google Scholar for funding trends
3. Generate detailed outline
4. Write full proposal in English

### Example 2 | 示例2

**User | 用户**:
```
research proposal
PhD proposal on "Machine Learning for DLC Coating Optimization"
Target: European research funding
Length: 8000 words
```

---

**For detailed writing guide | 详细写作指南**: [references/WRITING_STYLE_GUIDE.md](references/WRITING_STYLE_GUIDE.md)
