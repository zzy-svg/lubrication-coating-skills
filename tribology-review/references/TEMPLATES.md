# Project Templates | 项目模板

This document provides standardized templates for tribology literature review projects, including CLAUDE.md, IMPLEMENTATION_PLAN.md, and manuscript templates.

本文档为摩擦学文献综述项目提供标准化模板，包括CLAUDE.md、IMPLEMENTATION_PLAN.md和稿件模板。

---

## 1. CLAUDE.md Template | CLAUDE.md模板

### Complete CLAUDE.md Example | 完整CLAUDE.md示例

```markdown
# CLAUDE.md
# 润滑涂层文献综述 - Claude工作指南

This file provides guidelines for Claude Code when working on tribology literature review projects.
本文文件为Claude Code在摩擦学文献综述项目中提供工作指南。

---

## Project Context | 项目背景

**Review Topic | 综述主题**: [DLC Coatings for High-Temperature Applications]
**目标涂层 | Target Coatings**: DLC (a-C, a-C:H, ta-C)
**应用领域 | Application Area**: Aerospace, high-temperature environments
**预期页数 | Target Length**: 15-20 pages

---

## Terminology | 术语表

### Coating Types | 涂层类型
| Term | Abbreviation | Chinese | Description |
|------|--------------|---------|-------------|
| Diamond-Like Carbon | DLC | 类金刚石 | Amorphous carbon with sp³ bonding |
| Amorphous Carbon | a-C | 无定形碳 | Non-crystalline carbon |
| Hydrogenated DLC | a-C:H | 含氢类金刚石 | DLC containing hydrogen |
| Tetrahedral DLC | ta-C | 四面体类金刚石 | High sp³ content DLC |

### Performance Metrics | 性能指标
| Term | Symbol | Unit | Description |
|------|--------|------|-------------|
| Coefficient of Friction | COF (μ) | - | Friction coefficient |
| Wear Rate | WR | mm³/(N·m) | Volume loss per unit distance |
| Hardness | H | GPa | Coating hardness |
| Elastic Modulus | E | GPa | Young's modulus |

### Deposition Methods | 制备方法
| Term | Full Name | Chinese |
|------|-----------|---------|
| PVD | Physical Vapor Deposition | 物理气相沉积 |
| CVD | Chemical Vapor Deposition | 化学气相沉积 |
| PECVD | Plasma-Enhanced CVD | 等离子体增强CVD |
| Sputtering | Magnetron Sputtering | 磁控溅射 |
| Arc Deposition | Cathodic Arc Deposition | 阴极弧沉积 |

---

## Writing Style Guidelines | 写作风格指南

### Language Preference | 语言偏好
- **Section Headers**: English with Chinese in parentheses
- **Body Text**: English (for international publication)
- **Abstract**: Bilingual (EN first, then ZH)
- **Keywords**: English first, Chinese equivalent

### Hedging Language | 谨慎表达语言
**Use | 使用**:
- "may suggest"
- "appears to"
- "has demonstrated"
- "indicates that"
- "suggests potential for"
- "may be attributed to"

**Avoid | 避免**:
- "proves"
- "demonstrates conclusively"
- "is the best"
- "always"
- "never"

### Quantitative Reporting | 定量报告
**Always include | 始终包含**:
- Specific COF values with conditions
- Wear rate with units
- Hardness with measurement method
- Temperature ranges
- Sample sizes and test parameters

**Format | 格式**:
```markdown
"...achieved COF of 0.08 ± 0.02 under 10 N load at 0.1 m/s [23]."
"...showed wear rate of 2.5×10^-7 mm³/(N·m) on steel substrate [45]."
```

### Citation Format | 引用格式
**In-text citations | 文中引用**:
```markdown
Single: "...as reported [12]."
Multiple: "...demonstrated [12, 15, 23]."
Author-year: "...Li et al. [2023] proposed..."
```

**Reference list | 参考文献**:
```markdown
[1] Author, A., Author, B. (2023). Title of paper. Journal Name, Volume(Issue), Pages. DOI
```

---

## Key Metrics and Thresholds | 关键指标与阈值

### Performance Classification | 性能分类

| Metric | Excellent | Good | Acceptable | Poor |
|--------|-----------|------|------------|------|
| COF (dry) | < 0.05 | 0.05-0.15 | 0.15-0.30 | > 0.30 |
| Wear Rate | < 10^-7 | 10^-7-10^-6 | 10^-6-10^-5 | > 10^-5 |
| Hardness | > 40 GPa | 20-40 GPa | 10-20 GPa | < 10 GPa |
| Adhesion (Lc2) | > 70 N | 40-70 N | 20-40 N | < 20 N |

### Coating Temperature Limits | 涂层温度限制

| Coating | Max Temperature | Limiting Factor |
|---------|-----------------|-----------------|
| MoS₂ | 350°C | Oxidation |
| DLC (a-C:H) | 300°C | Hydrogen loss |
| DLC (ta-C) | 450°C | Graphitization |
| WS₂ | 500°C | Oxidation |
| h-BN | 900°C | Thermal stability |

---

## File Structure | 文件结构

```
project/
├── CLAUDE.md              # This file
├── IMPLEMENTATION_PLAN.md # Detailed plan
├── manuscript_draft.md    # Main manuscript
├── references/            # Reference management
│   ├── papers/           # PDF copies
│   └── notes.md         # Reading notes
└── figures/             # Figures and images
    ├── figure_1.png      # Coating structure
    ├── figure_2.png      # Friction curves
    └── figure_3.png      # Wear morphology
```

---

## Review Structure | 综述结构

```
1. Introduction (500-800 words)
   - 1.1 Background and motivation
   - 1.2 DLC coatings overview
   - 1.3 Review scope and objectives

2. DLC Coating Fundamentals (1000-1200 words)
   - 2.1 Classification and properties
   - 2.2 Deposition methods
   - 2.3 Characterization techniques

3. Tribological Performance (1500-2000 words)
   - 3.1 Friction behavior
   - 3.2 Wear mechanisms
   - 3.3 Environmental effects

4. High-Temperature Performance (1200-1500 words)
   - 4.1 Thermal stability
   - 4.2 Oxidation behavior
   - 4.3 Doping strategies

5. Applications (800-1000 words)
   - 5.1 Aerospace
   - 5.2 Automotive
   - 5.3 Other applications

6. Challenges and Future Directions (500-700 words)

7. Conclusion (200-300 words)

References: 80-120 citations
```

---

## Quality Standards | 质量标准

### Content Requirements | 内容要求
- [ ] 80-120 references (2019-2024 priority)
- [ ] 5+ comparison tables
- [ ] 5+ figures with detailed captions
- [ ] Quantitative data for all claims
- [ ] Discussion of limitations

### Language Requirements | 语言要求
- [ ] Consistent terminology (use glossary)
- [ ] Proper hedging language
- [ ] No absolute statements
- [ ] Clear transitions between sections

### Formatting Requirements | 格式要求
- [ ] Consistent heading hierarchy
- [ ] Proper citation format
- [ ] Detailed figure captions
- [ ] Cross-referencing between sections
```

---

## 2. IMPLEMENTATION_PLAN.md Template | IMPLEMENTATION_PLAN.md模板

```markdown
# IMPLEMENTATION_PLAN.md
# 润滑涂层文献综述实施计划

## Project Overview | 项目概述

| Field | Value |
|-------|-------|
| Review Topic | [DLC Coatings for High-Temperature Applications] |
| Start Date | [YYYY-MM-DD] |
| Target Completion | [YYYY-MM-DD] |
| Target Length | 15-20 pages (8000-10000 words) |

---

## Literature Collection Plan | 文献收集计划

### Phase 1: Initial Search (Days 1-2)
| Task | Source | Keywords | Target Papers |
|------|--------|----------|---------------|
| Broad overview | Google Scholar | "DLC coating review" | 30 |
| Coating types | ArXiv | "DLC a-C ta-C tribology" | 20 |
| High-temperature | Scholar | "DLC high temperature oxidation" | 15 |
| Deposition methods | Journals | "DLC PVD CVD review" | 15 |

### Phase 2: Focused Search (Days 3-4)
| Subtopic | Source | Keywords | Target Papers |
|----------|--------|----------|---------------|
| Thermal stability | WoS | "DLC thermal stability" | 20 |
| Doping effects | Scholar | "DLC Si N doping" | 15 |
| Wear mechanisms | Journals | "DLC wear mechanism" | 15 |
| Applications | Google | "DLC aerospace automotive" | 15 |

### Phase 3: Deep Dive (Days 5-6)
| Task | Details | Target |
|------|---------|--------|
| Citation tracking | Check "Cited by" for top 10 papers | +20 papers |
| Reference check | Review references of key reviews | +15 papers |
| Recent advances | 2023-2024 papers | +10 papers |

---

## Review Outline | 综述大纲

### Section 1: Introduction (500-800 words)
**Key Points | 关键点**:
- [ ] Define DLC and its significance
- [ ] State review scope
- [ ] Outline paper structure

### Section 2: DLC Fundamentals (1000-1200 words)
**Key Points | 关键点**:
- [ ] DLC classification (a-C, a-C:H, ta-C)
- [ ] Deposition methods overview
- [ ] Structure-property relationships

### Section 3: Tribological Performance (1500-2000 words)
**Key Points | 关键点**:
- [ ] Friction behavior by type
- [ ] Wear mechanisms
- [ ] Environmental effects

### Section 4: High-Temperature Behavior (1200-1500 words)
**Key Points | 关键点**:
- [ ] Thermal stability limits
- [ ] Oxidation mechanisms
- [ ] Doping strategies

### Section 5: Applications (800-1000 words)
**Key Points | 关键点**:
- [ ] Aerospace applications
- [ ] Automotive applications
- [ ] Emerging applications

### Section 6: Challenges & Future (500-700 words)
**Key Points | 关键点**:
- [ ] Current limitations
- [ ] Future research directions

### Section 7: Conclusion (200-300 words)
**Key Points | 关键点**:
- [ ] Summary of key findings
- [ ] Recommendations

---

## Tables and Figures | 表格与图表

### Required Tables | 必需表格
| # | Title | Content | Data Sources |
|---|-------|---------|--------------|
| T1 | DLC Classification | sp³, hardness, COF | Literature synthesis |
| T2 | Deposition Methods | Method, parameters, quality | Literature review |
| T3 | Performance Comparison | COF, wear rate by type | Experimental data |
| T4 | Doping Effects | Dopant, concentration, results | Literature review |
| T5 | Applications | Industry, coating, performance | Case studies |

### Required Figures | 必需图表
| # | Title | Type | Description |
|---|-------|------|-------------|
| F1 | DLC Structure | Schematic | sp²/sp³ bonding |
| F2 | COF vs Temperature | Graph | Performance curves |
| F3 | Wear Rate Comparison | Bar chart | By coating type |
| F4 | Tribological Mechanisms | Schematic | Wear process |
| F5 | Application Examples | Photos/images | Real applications |

---

## Milestones | 里程碑

| Milestone | Target Date | Status |
|-----------|-------------|--------|
| Literature collection complete | YYYY-MM-DD | [ ] |
| Outline approved | YYYY-MM-DD | [ ] |
| Sections 1-2 drafted | YYYY-MM-DD | [ ] |
| Sections 3-4 drafted | YYYY-MM-DD | [ ] |
| Sections 5-7 drafted | YYYY-MM-DD | [ ] |
| Tables and figures complete | YYYY-MM-DD | [ ] |
| First draft complete | YYYY-MM-DD | [ ] |
| Revision complete | YYYY-MM-DD | [ ] |
| Final submission | YYYY-MM-DD | [ ] |

---

## Progress Tracking | 进度追踪

### Week 1
- [ ] Literature search and collection
- [ ] Create literature matrix
- [ ] Develop detailed outline

### Week 2
- [ ] Write Sections 1-2
- [ ] Create initial tables
- [ ] Review and revise

### Week 3
- [ ] Write Sections 3-4
- [ ] Create figures
- [ ] Internal review

### Week 4
- [ ] Write Sections 5-7
- [ ] Complete tables/figures
- [ ] Final review and submission
```

---

## 3. Manuscript Draft Template | 稿件草稿模板

```markdown
# manuscript_draft.md
# [Title]: [Subtitle]

## Key Points | 关键发现
- [Bullet 1 - main finding]
- [Bullet 2 - second finding]
- [Bullet 3 - third finding]
- [Bullet 4 - additional key point]
- [Bullet 5 - fifth finding]

---

## Abstract | 摘要

[Diamond-Like Carbon (DLC) coatings have attracted significant attention for their exceptional tribological properties, including low coefficient of friction (COF) and high wear resistance. This review provides a comprehensive analysis of recent advances in DLC coatings for high-temperature applications, focusing on the effects of temperature on tribological performance, oxidation behavior, and stabilization strategies. The review covers DLC classification, deposition methods, and characterization techniques, followed by a detailed discussion of high-temperature performance including thermal stability, oxidation mechanisms, and doping approaches. Key findings indicate that ta-C coatings demonstrate superior thermal stability up to 450°C, while Si-doping effectively reduces oxidation rate and maintains low friction at elevated temperatures. Applications in aerospace, automotive, and industrial sectors are reviewed, highlighting the challenges and future research directions for high-temperature DLC coatings.]

**Keywords**: Diamond-like carbon; high-temperature tribology; oxidation resistance; coating; wear

---

## 1. Introduction | 引言

### 1.1 Background | 背景

[Content about tribology importance and DLC significance]

### 1.2 DLC Overview | DLC概述

[Overview of DLC coatings and their properties]

### 1.3 Review Scope | 综述范围

[Scope and objectives of this review]

---

## 2. DLC Fundamentals | DLC基础

### 2.1 Classification and Properties | 分类与性能

| DLC Type | sp³ Content | Hardness | COF | Applications |
|-----------|-------------|----------|-----|--------------|
| a-C | 40-70% | 20-30 GPa | 0.10-0.20 | General |
| a-C:H | 50-80% | 10-25 GPa | 0.05-0.15 | Automotive |
| ta-C | 70-90% | 40-80 GPa | 0.05-0.10 | Cutting tools |

### 2.2 Deposition Methods | 制备方法

[PVD, CVD methods and parameters]

### 2.3 Characterization | 表征方法

[Characterization techniques and standards]

---

## 3. Tribological Performance | 摩擦学性能

### 3.1 Friction Behavior | 摩擦行为

### 3.2 Wear Mechanisms | 磨损机制

### 3.3 Environmental Effects | 环境影响

---

## 4. High-Temperature Performance | 高温性能

### 4.1 Thermal Stability | 热稳定性

### 4.2 Oxidation Behavior | 氧化行为

### 4.3 Doping Strategies | 掺杂策略

---

## 5. Applications | 应用

### 5.1 Aerospace | 航空航天

### 5.2 Automotive | 汽车工业

### 5.3 Other Applications | 其他应用

---

## 6. Challenges and Future Directions | 挑战与未来方向

---

## 7. Conclusion | 结论

---

## References | 参考文献

[1] Author, A. et al. (2023). Title. Journal, Volume, Pages.
[2] Author, B. et al. (2022). Title. Journal, Volume, Pages.
...
```

---

**See also | 参见**:
- [WORKFLOW.md](WORKFLOW.md) - Complete workflow
- [QUALITY_CHECKLIST.md](QUALITY_CHECKLIST.md) - Quality requirements
