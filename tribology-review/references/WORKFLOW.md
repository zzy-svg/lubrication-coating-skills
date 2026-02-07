# 7-Phase Literature Review Workflow | 七阶段文献综述工作流

This document details the systematic 7-phase workflow for writing comprehensive literature reviews in lubrication coating materials and tribology research.

本文档详细说明了润滑涂层材料和摩擦学研究领域撰写综合文献综述的系统性七阶段工作流。

---

## Phase 1: Project Initialization | 阶段1：项目初始化

### 创建项目结构 | Create Project Structure

```
project_root/
├── CLAUDE.md              # 写作指南和术语规范
├── IMPLEMENTATION_PLAN.md # 分阶段执行计划
├── manuscript_draft.md   # 主稿件
└── figures/               # 图表占位符
```

### 操作步骤 | Actions

1. **Create CLAUDE.md** from template (see [TEMPLATES.md](TEMPLATES.md))
   - 定义涂层术语和缩写 | Define coating terminology and abbreviations
   - 设定写作风格和格式规范 | Set writing style and formatting guidelines
   - 指定关键指标和单位 | Specify key metrics and units

2. **Create IMPLEMENTATION_PLAN.md**
   - 设定综述范围和目标 | Define review scope and objectives
   - 规划各章节内容 | Plan section content
   - 设定时间节点和里程碑 | Set timeline and milestones

3. **Initialize manuscript_draft.md**
   - 创建标准综述结构模板 | Create standard review structure template
   - 添加图表占位符 | Add figure and table placeholders

### Example | 示例

```markdown
# DLC Coatings for High-Temperature Applications: A Comprehensive Review

## CLAUDE.md

### Terminology | 术语
- DLC: Diamond-Like Carbon
- a-C: Amorphous Carbon
- a-C:H: Hydrogenated Amorphous Carbon
- ta-C: Tetrahedral Amorphous Carbon
- COF: Coefficient of Friction
- WR: Wear Rate

### Writing Style | 写作风格
- Use hedging language: "may", "suggests", "demonstrated"
- Include quantitative data: COF values, wear rates, hardness
- Cite recent literature: 2019-2024 priority
```

---

## Phase 2: Literature Collection | 阶段2：文献收集

### 数据源 | Data Sources

#### 2.1 ArXiv MCP (Latest Materials Research)

**最佳用途 | Best for**: Cutting-edge synthesis methods, ML applications, preprints

**搜索策略 | Search Strategy**:
```
Query: "[coating type] AND (tribology OR friction OR wear)"
Categories: cond-mat.mtrl-sci, physics.app-ph
Date: Last 3-5 years
Max results: 50-100 per query
```

**示例查询 | Example Queries**:
- "DLC coating tribology machine learning"
- "MoS2 solid lubricant deposition"
- "self-lubricating coating high temperature"
- "tribological properties DLC"
- "wear resistance coating synthesis"

**工作流 | Workflow**:
1. Use `search_papers` with topic keywords
2. Review titles and abstracts for relevance
3. Use `download_paper` for key papers
4. Use `read_paper` to extract method details and performance data

#### 2.2 Scholar MCP Server (Comprehensive Coverage)

**最佳用途 | Best for**: Citation tracking, journal articles, broad search

**搜索策略 | Search Strategy**:
```bash
# Google Scholar Advanced Search
allintitle: "DLC coating" AND friction
allintitle: "solid lubricant" AND wear
author: "Lastname, Firstname"
```

**示例查询 | Example Queries**:
```markdown
# 涂层分类搜索
"solid lubricant coating" MoS2 WS2 h-BN
"DLC coating" hydrogenated tetrahedral
"self-lubricating" composite coating

# 性能指标搜索
"coefficient of friction" DLC temperature
"wear rate" coating durability
"tribological properties" review

# 应用领域搜索
"coating" aerospace automotive biomedical
"cutting tool" DLC coating performance
```

#### 2.3 Specific Journal Search | 特定期刊搜索

| Journal | Focus Area | Impact Factor |
|---------|------------|---------------|
| Tribology International | Fundamental tribology | ~6.5 |
| Wear | Wear mechanisms | ~5.0 |
| Surface & Coatings Technology | Industrial applications | ~5.3 |
| Tribology Letters | Rapid communications | ~3.0 |
| Coatings (MDPI) | Coating science | ~3.5 |
| Friction | Tribology research | ~4.0 |

### 文献矩阵 | Literature Matrix

创建文献分类矩阵：

| Category | Subcategory | Key Papers | Count | Source |
|----------|-------------|------------|-------|--------|
| DLC Coatings | a-C:H | [refs] | N | ArXiv/Scholar |
| DLC Coatings | Doping (Si, N) | [refs] | N | Scholar |
| Solid Lubricants | MoS2 | [refs] | N | ArXiv |
| Solid Lubricants | WS2 | [refs] | N | Scholar |
| Solid Lubricants | h-BN/Graphene | [refs] | N | ArXiv |
| Deposition Methods | PVD/Sputtering | [refs] | N | Journals |
| Deposition Methods | CVD | [refs] | N | Journals |
| Testing Methods | COF Measurement | [refs] | N | Standards |
| Testing Methods | Wear Testing | [refs] | N | Standards |
| Applications | Aerospace | [refs] | N | Scholar |
| Applications | Automotive | [refs] | N | Scholar |
| Applications | Biomedical | [refs] | N | Scholar |

### 差距分析 | Gap Analysis

After initial collection, identify gaps:
- [ ] Missing time periods or recent advances
- [ ] Uncovered subtopics or applications
- [ ] Limited comparative studies
- [ ] Insufficient performance data

Conduct targeted searches to fill gaps.

---

## Phase 3: Outline Development | 阶段3：大纲制定

### 标准结构 | Standard Structure

```markdown
# [Title]: Comprehensive Review

## Key Points (3-5 bullets)

## Abstract (200-300 words)

## 1. Introduction
### 1.1 Background and Motivation
### 1.2 Tribological Importance
### 1.3 Review Scope and Objectives

## 2. Materials and Methods
### 2.1 Coating Classification
### 2.2 Deposition Techniques
### 2.3 Characterization Methods

## 3. Results and Discussion
### 3.1 [Category 1]
### 3.2 [Category 2]
### 3.3 Comparative Analysis

## 4. Applications

## 5. Challenges and Future Directions

## 6. Conclusion

## References
```

### 大纲输出 | Output

更新 IMPLEMENTATION_PLAN.md 包含：
- 各章节详细标题
- 映射到章节的论文
- 计划表格和图表
- 时间节点

---

## Phase 4: Section Writing | 阶段4：章节撰写

### 每个主要章节遵循以下步骤：

1. **Write introduction** (1-2 paragraphs on motivation)
2. **Describe methods/coatings** using standard template
3. **Add performance data** with consistent metrics
4. **Write limitations** paragraph
5. **Create comparison table**
6. **Update references**

### 涂层描述模板 | Coating Description Template

```markdown
### 3.X [Coating Category]

[1-2 paragraph introduction with motivation | 1-2段动机介绍]

**[Coating Name]:** [Author] et al. [year] proposed [method], which features:
- [Key composition/structure 1]
- [Key composition/structure 2]

Achieved COF of 0.XX and wear rate of X×10^-X mm³/Nm on [substrate].

**Limitations:** Despite advantages, [category] coatings face:
(1) [limitation 1]
(2) [limitation 2]
```

### 进度追踪 | Progress Tracking

使用 TodoWrite 追踪每个章节：
```markdown
- [ ] Section 3.1: DLC Coatings
- [ ] Section 3.2: Solid Lubricants
- [ ] Section 3.3: Composite Coatings
- [ ] Section 4: Applications
```

---

## Phase 5: Tables and Figures | 阶段5：表格与图表

### 必需表格 | Required Tables

| Table # | Title | Content |
|---------|-------|---------|
| Table 1 | Public Datasets | Coating types, substrates, test conditions |
| Table 2 | Method Comparison | COF, wear rate, hardness, temperature range |
| Table 3 | Deposition Methods | Technique, parameters, advantages |
| Table 4 | Applications | Industry, coating type, performance |

### 图表占位符 | Figure Placeholders

- **Figure 1**: Review overview/taxonomy (涂层分类图)
- **Figure 2**: Method evolution timeline (方法发展时间线)
- **Figure 3**: Performance comparison chart (性能对比图)
- **Figure 4**: Mechanism schematic (机制示意图)
- **Figure 5**: Application examples (应用实例)

### Figure Caption Template | 图表描述模板

```markdown
![Figure X](figures/figure_x.png)

**Figure X.** [Title]. [Brief description of what the figure shows, including key findings and any notable trends observed in the data].
```

---

## Phase 6: Quality Assurance | 阶段6：质量保证

### 结构检查 | Structure Check

- [ ] Key Points present after title
- [ ] All sections have summary tables
- [ ] Consistent heading hierarchy
- [ ] Proper citation format throughout

### 内容检查 | Content Check

- [ ] All major coating types covered
- [ ] Quantitative data included (COF, wear rate)
- [ ] Recent literature included (2019-2024)
- [ ] Limitations discussed
- [ ] Future directions articulated

### 语言检查 | Language Check

- [ ] Hedging language used appropriately
- [ ] Terminology consistent (use CLAUDE.md glossary)
- [ ] Transitions smooth between sections
- [ ] No absolute statements ("best", "perfect")

### 引用检查 | Reference Check

- [ ] 80-120 references
- [ ] Recent literature included
- [ ] Organized by topic
- [ ] Proper citation format

---

## Phase 7: Incremental Updates | 阶段7：增量更新

当新文献出现时 | When new literature becomes available:

1. **Categorize** new papers
2. **Update CLAUDE.md** reference sources
3. **Update IMPLEMENTATION_PLAN.md** with new stage
4. **Identify insertion points** in manuscript
5. **Update sections** with new methods
6. **Add new sections** if new paradigm emerges
7. **Update tables** with new data
8. **Expand references**

### 版本控制 | Version Control

```markdown
## Change Log | 变更日志
### [Date] - v1.X
- Added Section 3.X [New Category]
- Updated Table 2 with N new methods
- Added references #XX-#YY
```

---

## Quick Reference | 快速参考

| Phase | Main Task | Key Outputs |
|-------|-----------|-------------|
| 1 | Initialize | CLAUDE.md, IMPLEMENTATION_PLAN.md |
| 2 | Collect | Literature matrix, gap analysis |
| 3 | Outline | Detailed section structure |
| 4 | Write | Section drafts with citations |
| 5 | Visualize | Tables, figures, captions |
| 6 | Verify | Checklist completion |
| 7 | Update | Incremental improvements |

---

**See also | 参见**:
- [DOMAINS.md](DOMAINS.md) - Coating categories
- [METRICS.md](METRICS.md) - Performance metrics
- [TEMPLATES.md](TEMPLATES.md) - File templates
